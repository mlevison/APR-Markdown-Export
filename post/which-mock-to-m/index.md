---
title: "Which Mock to Mock with? JMock? RMock? EasyMock?"
date: "2007-07-18"
categories: 
  - "software-development"
coverImage: "test-xs.jpg"
---

![a pencil sitting on a test bubble sheet - image licensed from Photodune](src/content/blog/which-mock-to-m/images/test-xs.jpg) After years of making half hearted attempts at test driven development I’m finally taking the plunge and doing it properly. After only a few days of doing TDD I got tired of implementing interfaces long hand. It’s especially annoying since you typically only care about one or two methods in the object but have to fill them all out. The trouble comes for the reader of your code who can’t tell immediately what return values you care about and which ones are the default values that were generated for you. So I began looking for mocking framework. My only criteria must work with Java 1.4 – so no annotations or generics. Based on a thread in the JUnit mailing list Mock Framework reviews ([https://tech.groups.yahoo.com/group/junit/message/19315](https://tech.groups.yahoo.com/group/junit/message/19315)) I decided to give JMock and RMock a try.

## [Easy Mock](https://easymock.org/)

Why didn’t I try using EasyMock 1.2? Its style just doesn’t appeal to me. Like [Vi](https://en.wikipedia.org/wiki/Vi) it is stateful/modal i.e. you have to do things in a particular sequence and you can’t always tell from reading the code what mode your in. In particular there are setup and replay modes. First you build your mock, and then you flip the replay bit. Now calls to the method under test will be verified for conformance. I find this deeply weird. I always hated vi because if you stepped away from your machine and came back you could never quite be sure what mode you were in: command mode or text entry mode. EasyMock suffers the same problem – the replay call can be anywhere (think abstract test cases) – the reader has to guess whether the Mock is ready for use.

## [RMock](https://rmock.sourceforge.net)

This one really appealed to me – a modern mock tool that still supported Java 1.4. In addition it didn’t used strings to find methods it used the methods themselves. Fantastic I thought. On paper this approach appealed to me. Then I tried to write code:

```
// BTW The example code is dumbed down to avoid introducing other classes and so tests something that is completely pointless. Trust that the code this comes from has a point 
IRead somethingRead = (IRead) mock(IRead.class);
somethingRead.getAttributes();
modify().returnValue(ATTRIBUTES);

startVerification();
Attributes attributes = somethingRead.getAttributes();
assertEquals(ATTRIBUTES, attributes);
```

The first line makes sense, but it’s the second where things get a little weird – we call somethingRead.getAttributes() not to execute but to tell RMock that we wish to change it. In line three we call a Multiplicity modifier to change the return value. Finally we call startVerification() to be allowed to make use of our mock. And there we are back in modal land again. I know some people like Vi but its not me. Just in case I’m out to lunch I tried sharing this code with my team – they all found it hard to wrap their heads around but would use it if I asked nicely. They’re all too young to know what Vi is. One other detail your tests must be derived from RMock’s test case.

## [JMock](https://www.jmock.org)

N.B. all my remarks are about [JMock 1.2](https://www.jmock.org/download.html) - the last version to support Java 1.4. It’s funny some times how hard you resist something even when it comes with the recommendation of people you respect. Both JB Raingsberger and Bob Martin have remarked that they currently use JMock yet I wasn’t sold. However after finding RMock to confusing for my tastes I thought I better give JMock a try. Here’s the code snippet:

```
Mock mockRead = mock(IRead.class);
IRead somethingRead = (IRead) mockRead.proxy();
mockRead.expects(atMostOnce()).method(“getAttributes”).will(returnValue(ATTRIBUTES));
Attributes attributes = somethingRead.getAttributes();
assertEquals(ATTRIBUTES, attributes);
```

JMock creates two classes the Mock “manager” - mockRead and the proxy class - somethingRead (i.e. the class under simulation). The readability of the third line is what really appeals to me. I appreciate that mockRead expects that getAttributes will be called at most once and will return the value Attributes. I also like that the mock is always ready for use so there won’t be any issues looking for missing startVerification/verify calls.

### annoyances

- The string based approach to identifying methods will cause us very interesting surprises when the interface items are renamed (this is happens quite a bit because the API’s we’re consuming are still fairly young). N.B. [JMock 2.0](https://www.jmock.org/getting-started.html) appears to address this issue.
- The stock constraints for expects are a bit thin atMostOnce, atLeastOnce, never, once – missing support for don’t care and a specific number of calls. (In my example I don’t care – but I can’t easily communicate that to the reader. RMock definitely had more constraints.
- The language for testing arguments passed to a mock method is a bit limiting so I’m forced to create a custom constraints class to test simply things. In particular to do this: EXPECTED\_NAME.equals(((Folder) o).getName()) - I was forced to create a custom class when casting the arg is all I really wanted.
- Can't mock classes - occasionally I would like to mock something that's an abstract class. _I think that both JMock 2.0 and RMock support this._

Which Mock framework did you choose? Why?

Image via: [https://photodune.net/](https://photodune.net/)
