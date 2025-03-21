---
title: "Unit Testing in JavaScript"
date: "2008-11-25"
categories: 
  - "software-development"
  - "tdd"
tags: 
  - "javascript"
  - "jsunit"
  - "stackoverflow"
  - "test-driven-development"
  - "unit-testing"
coverImage: "hacking-codes-xs.jpg"
excerpt: 'Last week a colleague asked for my help finding better unit test tools for Java Script.'
---

![Hacking codes - image licensed from Photodune](src/content/blog/unit-testing-in-javascript/images/hacking-codes-xs.jpg)

Last week a colleague asked for my help finding better unit test tools for Java Script. He's done some digging on the state of the art with JavaScript unit tests and finds the whole lot wanting. His discoveries:

<table class="postTable" border="2" width="736" cellspacing="0" cellpadding="2"><tbody><tr><td valign="top" width="133"><strong>Tool</strong></td><td valign="top" width="233"><strong>Pros</strong></td><td valign="top" width="367"><strong>Cons</strong></td></tr><tr><td valign="top" width="133"><strong><a href="https://www.jsunit.net/">Jsunit</a></strong>: we already use it for some of our js code.</td><td valign="top" width="233"><ul><li>can be invoked from an ant build file</li><li>launches browser to run the tests</li><li>eclipse plug-in</li><li><a href="https://tech.groups.yahoo.com/group/jsunit/" target="_blank" rel="noopener noreferrer">Mailing list</a> is still active</li></ul></td><td valign="top" width="367"><ul><li>launches browser to run the tests</li><li>Does not support js file to write the unit test code: it has to embedded inside a html file</li><li>it has not be updated for a couple of years<em>&nbsp; - while there hasn't been a release changes have been made to the source repository (perhaps minor) in the past year.</em></li></ul></td></tr><tr><td valign="top" width="133"><a href="https://code.google.com/p/rhinounit/">rhinounit</a></td><td valign="top" width="233"><ul><li>ant driven</li><li>supports js file</li><li>very simple to use</li></ul></td><td valign="top" width="367"><ul><li>Simulation of JavaScript engine: not advanced enough to support our code: I tried to run test code working with jsunit: I encountered issue when loading our common JavaScript files.</li></ul></td></tr><tr><td valign="top" width="134">crosscheck: Note: Crosscheck wasn't tested with any code.</td><td valign="top" width="233"><ul><li>Can invoked from ant build file</li><li>Simulates real browser behaviour</li></ul></td><td valign="top" width="367"><ul><li>Simulation of JavaScript engine from a limited number of browser versions.</li><li>No activity for 2 years: it does not support versions 2.x nor 3.x from Firefox.</li></ul></td></tr><tr><td valign="top" width="134"><a href="https://code.google.com/p/jsspec/">jsspec</a></td><td valign="top" width="233"><ul><li>Runs on actual browser</li></ul></td><td valign="top" width="367"><ul><li>JavaScript only framework: cannot be called from ant build file</li></ul></td></tr><tr><td valign="top" width="134">jspec (no website - just a source tree)</td><td valign="top" width="233"><ul><li>Runs on actual browser</li></ul></td><td valign="top" width="367"><ul><li>Does not seem to support our code:&nbsp; I tried to run test code running with js unit: I encountered issue when loading our common JavaScript files.</li><li>JavaScript only framework: cannot be called from ant build file</li></ul></td></tr><tr><td valign="top" width="134">Screw.unit (<a href="https://github.com/nkallen/screw-unit/tree/master">docs</a>) Note: Not tested but it is very similar to jsspec and jspec.</td><td valign="top" width="233"><ul><li>Runs on actual browser</li></ul></td><td valign="top" width="367"><ul><li>JavaScript only framework: cannot be called from ant build file</li></ul></td></tr></tbody></table>

So it seems to him that Jsunit is the only choice we have. It is not perfect though because it does not provide an easy way to apply  the TDD process for the following reasons:

- It does not provide a simple and integrated way to run JavaScript unit test
- It forces you to write the unit tests in a html file instead of a .js file.
- It forces you to have a local installation of the jsunit framework in order to avoid absolute hard coded path to reference js unit files.

As a consequence, you have to switch back and forth from you IDE and all the browsers we want to support while "TDDing" in JavaScript. It is feasible but doesn't seem very effective.

I tried asking about this on [StackOverflow](external:https://stackoverflow.com/questions/300855/javascript-unit-test-tools-for-tdd) generated some interesting answers:

- Look at the Dojo Object Harness (DOH) unit test framework which is pretty much framework independent harness for JavaScript unit testing and doesn't have any Dojo dependencies. I found a very good description of it at [Medrix Observations: Dojo D.O.H. Unit Testing](external:https://blog.medryx.org/2008/06/08/dojo-doh-unit-testing/). Interestingly we have at least one team (Yvon's) that is experimenting with Dojo. (_got several recommendations for this_)
- Apparently MochiKit - yet another library has a framework called [SimpleTest](external:https://medium.com/leos-tech-blog/interesting-open-source-surprises-87fe2ed81ec0) buried inside it.

Asking on the [Test Driven Mailing](external:https://tech.groups.yahoo.com/group/testdrivendevelopment) List got another batch of answers:

- [QUnit](external:https://qunitjs.com) from jQuery (_got several recommendations for this_)
- [Mocking tool](external:https://jsmock.sourceforge.net/) for JavaScript
- Use GWT and do all your work in Java

In addition two people didn't answer the question directly but instead sent my in the direction of some books:

- [Secrets of the JavaScript Ninja](external:https://www.manning.com/books/secrets-of-the-javascript-ninja) by the project lead for jQuery (which will have a chapter on Unit Testing)

#### Conclusions

There isn't one good place to ask JavaScript/Unit Testing questions. The best so far seems [StackOverflow.com](external:https://stackoverflow.com/questions/tagged/javascript) seems to be the only real option.

Of the Unit Test Frameworks the real options seem to be:

- [JSunit](external:https://www.jsunit.net/)
- The Dojo Object Harness (DOH) unit test framework
- [QUnit](external:https://qunitjs.com) from jQuery
- YUI Test: see [YUI Test - The New Kid on Block](external:https://sites.google.com/site/tedhusted/posts/yui-test---the-new-kid-on-block)

I also did some digging for Mock Frameworks and have only come up with a list of tools:

- [JSMock](external:https://jsmock.sourceforge.net/) - JSMock provides expectation recording and matching, and has the ability to return, throw, and stub on object method calls
- Jack - The project aims to help developers write short and readable JavaScript tests.
- [MockMe](external:https://johanneslink.net/projects/mockme.html) - written because of [Johanne's](external:https://blog.johanneslink.net/2008/08/08/ajax-travelogue-part-6-mocking-in-javascript/) [dissatisfaction](external:https://blog.johanneslink.net/2008/08/09/ajax-travelogue-part-7-mockme/) with other JavaScript Mock tools.
- [QMock](external:https://code.google.com/p/qmock/) - very new

There is some good writing that will give you a flavour of TDD with Javascript:

- [Test Driven AJAX](external:https://www.slideshare.net/jlink/agile08-test-driven-ajax) a presentation from Agile 2008 (long but through)
- [TDD and Javascript with JsMock](external:https://www.pathf.com/blogs/2006/11/tdd_and_javascr/)
- [Test Driven Javascript](external:https://www.testdrivenjavascript.com/Practice/5.aspx)
- [TDD and Javascript with JsMock](external:https://www.techtarget.com/searchsoftwarequality/definition/mock-object)

Best ongoing sources: Pathfinder Blog and [Ajaxian](external:https://ajaxian.com/by/topic/testing) seem to be good reading.

What tools did I miss? Are there any good JavaScript mailing lists where the participants discuss TDD?

Image via: [https://photodune.net/](external:https://photodune.net/)
