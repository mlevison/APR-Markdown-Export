---
title: "Minimalist Coding Style"
date: "2008-07-21"
categories: 
  - "software-development"
coverImage: "modern-office-xs.jpg"
excerpt: '- Why do you need this boolean named retVal? Could it be eliminated the use of early'
---

![modern office - image licensed from Photodune](src/content/blog/minimalist-coding-style/images/modern-office-xs.jpg) “Perfection is achieved, not when there is nothing more to add, but when there is nothing left to take away” - **[Antoine de Saint  Exupéry](external:https://en.wikipedia.org/wiki/Antoine_de_Saint_Exup%C3%A9ry)**. If you’ve ever invited me do some pair programming with you, you probably have a good idea what this quote is all about. I often wind up asking questions like:

- Why do you need this boolean named retVal? Could it be eliminated the use of early return statements?
- Is the else clause in this if statement necessary? Could it be avoided with a return statement? Or break/continue in a loop?
- I noticed that this method has parts that are nested five levels of braces deep. Is there anything we can do to reduce that?

Two recent posts [Spartan Programming](external:https://blog.codinghorror.com/spartan-programming/) (Jeff Atwood Coding Horror) taken from the [Spartan Programming page on the Technion Wiki](external:https://ssdl-wiki.cs.technion.ac.il/wiki/index.php/Spartan_programming) and [Life After If, For and Switch](external:https://www.hanselman.com/blog/back-to-basics-life-after-if-for-and-switch-like-a-data-structures-reminder) (Scott Hansleman Computerzen), have reminded me of this subject.

Most of the Spartan ideas make sense to me:

- [Minimize depth of nesting of control structures](external:https://ssdl-wiki.cs.technion.ac.il/wiki/index.php/Horizontal_complexity%2C_spartan_reduction_of)
- [Minimize the number of lines occupied](external:https://ssdl-wiki.cs.technion.ac.il/wiki/index.php/Vertical_complexity%2C_spartan_reduction_of) – the idea being its easier to make sense of a method if its all on one screen. I would prefer that most methods be < 10 lines long. _Some people read this suggestion to mean all blank lines should eliminated. I would disagree preferring to use blank lines like paragraph breaks, they indicate we’re changing gears._
- Minimize [Token](external:https://ssdl-wiki.cs.technion.ac.il/wiki/index.php/Token_count%2C_spartan_reduction_of) and [Character](external:https://ssdl-wiki.cs.technion.ac.il/wiki/index.php/Character_count%2C_spartan_reduction_of) Count suggest removing braces etc. – i.e. remove every non-essential character. _I think these measures can be harmful and wouldn’t use them._
- Minimize the number of [Parameters](external:https://ssdl-wiki.cs.technion.ac.il/wiki/index.php/Parameters%2C_spartan_reduction_of) to a method and avoid the use of out params.
- Reduce the number of [Variables](external:https://ssdl-wiki.cs.technion.ac.il/wiki/index.php/Variables%2C_spartan_reduction_of) – a number of excellent techniques are shown. I disagree with only two: the use of ternary operator and encouraging the use of very [terse variable names](external:https://ssdl-wiki.cs.technion.ac.il/wiki/index.php/Terse_variable_naming).

Jeff Atwood codifies the **frugal use of variables:**

- Minimize _number_ of variables. Inline variables which are used only once. Take advantage of `foreach` loops.
- Minimize _visibility_ of variables and other identifiers. Define variables at the smallest possible scope.
- Minimize _accessibility_ of variables. Prefer the greater encapsulation of `private` variables.
- Minimize _variability_ of variables. Strive to make variables `final` in Java and `const` in C++. Use annotations or restrictions whenever possible. _**The only caveat here – having tried making both parameters and local variables final I found no benefit and so gave up.**_
- Minimize _lifetime_ of variables. Prefer ephemeral variables to longer lived ones. Avoid persistent variables such as files.
- Minimize _names_ of variables. Short-lived, tightly scoped variables can [use concise, terse names](external:https://ssdl-wiki.cs.technion.ac.il/wiki/index.php/Terse_variable_naming). **_On this we completely disagree._**
- Minimize _use of array_ variables. Replace them with collections provided by your standard libraries.

My additional rules:

- **Booleans** make bad parameters. If you have method that has doStuff(realParam, true, false) – how does someone reading the calling know what true and false mean. At the very minimum use enums with meaningful names.
- One letter variable names like i,j,k and e come from the early days of Fortran where variables were 1-6 characters long. With so few characters its not surprise that common convention dictated that i,j,k were loop/index variables. We’ve come a long since then – use names that while concise get the point across.
- Rather than for(int index = 0; index < size(); index++) use Java (or .NET’s) foreach. They save an unnecessary indexing variable.
- Check arguments at the start of any public or package level method and after that assume they’re right. You can find libraries to simplify this for you (I’ve written one at work) and if you don’t work with me see: “[I take exception to that argument](external:https://www.codeproject.com/Articles/9037/I-take-exception-to-that-argument)” on Code Project.
- Minimize the use of instanceof – as your class structure grows these will be hard to maintain. More on this in up coming post.
- The if/switch statement you don’t write is one you don’t have to test.

My cardinal rule: Always program as if the person maintaining your code six months from now is an axe murder. The last thing you want to do is give him (or her) an excuse to come visit you in frustration.

So next you invite me to pair program at least you have an idea about some of the questions I will ask.

Image via: [https://photodune.net/](external:https://photodune.net/)
