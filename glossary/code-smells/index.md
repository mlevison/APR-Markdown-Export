---
title: "Code Smells"
date: "2024-10-10"
relatedTerms: 'technical-debt'
---

A **code smell** is a hint that something might be wrong in your codebase. A smell isn't always a problem, rather it’s a hint that a further look is warranted. Code smells are a clue that says more time is needed to examine this area of the code.

They originated from one of the early Agile books, _Refactoring_ by Martin Fowler (so important that it got a second edition). Many code smells are simple to describe: Mysterious Name, Duplicated Code, Long Function, Long Parameter List and Long Class.

The descriptions below are a mix of my own and some from [The Code Smells Catalogue](https://github.com/Luzkan/smells/blob/main/README.md), which is an attempt to create a complete catalog of all code smells. I’ve listed only a subset here.

### Bloaters

They make the code base harder to read, follow and modify by adding bulk.

| **Smell** | **Description** |
| --- | --- |
| [Data Clump](https://luzkan.github.io/smells/data-clump) | Data Clumps refer to a situation in which a few variables are passed around many times in the codebase instead of being packed into a separate object. |
| [Long Method](https://luzkan.github.io/smells/long-method) | One of the most apparent complications developers can encounter in the code is the length of a method. The more lines of code a function has, the more the developer has to strain himself mentally to comprehend what the particular block of code does thoroughly. |
| [Long Parameter List](https://luzkan.github.io/smells/long-parameter-list) | This is another code smell at the same abstraction level as Long Method which usually occurs when three, four, or more parameters are given as input for a single method. Basically, the longer the parameter list, the harder it is to understand. |
| [Null Check](https://luzkan.github.io/smells/null-check) | Null check is widespread everywhere because the programming languages allow it. It causes a multitude of undefined or null checks everywhere: in guard checks, in condition blocks, and verifications clauses. Instead, special objects could be created that implement the missing-event behavior, errors could be thrown and caught, and many duplications would be removed. Even an anecdote sometimes appears on discussion forums that the inventor of the null reference, Tony Hoare (also known as the creator of the QuickSort algorithm), apologizes for its invention and calls it a _billion-dollar mistake_. |
| [Primitive Obsession](https://luzkan.github.io/smells/primitive-obsession) | Whenever a variable that is just a simple string, or an int simulates being a more abstract concept, which could be an object, we encounter a _Primitive Obsession_ code smell. |

### Object-Oriented or Functional Abusers

Misuse of OO or Functional principles.

| **Smell** | **Description** |
| --- | --- |
| [Conditional Complexity](https://luzkan.github.io/smells/conditional-complexity) | Nested switch or if statements; a series of successive if statements. _This preceding statement is itself an example._ |
| [Inappropriate Static](https://luzkan.github.io/smells/inappropriate-static) | Static methods and class fields are the OO equivalent of Global Data. They allow global access to themselves, increasing coupling and reducing testability. There are clearly cases -  Math.max() for example - where a static is useful. They're few and far between. |
| [Refused Bequest](https://luzkan.github.io/smells/refused-bequest) | Whenever a subclass inherits from a parent but only uses a subset of the implemented parent methods, that is called _Refused Bequest_. |
| [Side Effect](https://luzkan.github.io/smells/side-effects) | A method does more than its name promises, changing a variable/state that isn't part of its named purpose. Eg. a setAmount() that changes a date field. |
| [Temporary Field](https://luzkan.github.io/smells/temporary-field) | A variable on a class or object that is only initialized and used in particular circumstances, i.e. by one or two methods. |

### Change Preventers

| **Smell** | **Description** |
| --- | --- |
| [Divergent Change](https://luzkan.github.io/smells/divergent-change) | If adding a simple feature makes the developer change many seemingly unrelated methods inside a class, that indicates the _Divergent Change_ code smell. |
| [Flag Argument](https://luzkan.github.io/smells/flag-argument)
(aka Boolean argument) | Code smell occurs when a method requires a boolean or similar flag argument to control its behavior. The flag makes it difficult for the reader to follow the code without digging into the implementation. It also indicates that the method may have too many responsibilities. |
| [Shotgun Surgery](https://luzkan.github.io/smells/shotgun-surgery) | Similar to Divergent Change but with a broader spectrum, the smell symptom of the Shotgun Surgery code is detected by the unnecessary requirement of changing multiple different classes to introduce a single modification. Things like that can happen with the failure to use the correct design pattern for the given system. This expansion of functionality can lead to an easy miss (and thus introduce a bug) if these small changes are all over the place and they are hard to find. |

### Dispensables

| **Smell** | **Description** |
| --- | --- |
| Dead Code | Unreachable code |
| Duplicated Code | Possibly the worst smell |
| [Speculative Generality](https://luzkan.github.io/smells/speculative-generality) | Developers are humans, and humans are bad guessers. Developers tend to create additional features in preparation for the future, guessing that they will be useful, but that time never came. |

### Couplers

| **Smell** | **Discussion** |
| --- | --- |
| [Fate over Action](https://luzkan.github.io/smells/fate-over-action)
(replaces Fowler's original Data Class) | In the original definition a class with only Getters/Setters was considered a Data Class. A Data Class that allows others to change its contents is a source of many errors since we may discover the data changed over the life of the program without knowing how, when or why.

Use of Final/ReadOnly Data transfer objects (i.e. no setters), sidesteps these problems.

Fate over action focuses on the challenge where outside classes call setters on a class, leaving the receiver with no control of its fate. |
| [Feature Envy](https://luzkan.github.io/smells/feature-envy) | If a method inside a class manipulates more features (be it fields or methods) of another class more than from its own, then this method has a _Feature Envy_. |
| [Message Chain](https://luzkan.github.io/smells/message-chain) | Suppose that class A requires data from class D, but to retrieve those data, it has to make unnecessary calls to class B sequentially and then C to get it. This function sequencing is called Message Chain code smell. Long sequences of methods calls indicate hidden dependencies by being intermediaries. A sequence of temporary variables could have also hidden the sequence of methods. The problem with this smell is that any change in the intermediate relationship causes the client to have to change. |
| [Middle Man](https://luzkan.github.io/smells/middle-man) | The class that only performs delegation work to other classes is called a _Middle Man_. This is the opposite of the Message Chains. Encapsulation (hiding internal details) in the world of Object-Oriented Programming is a typical pattern. However, the problem arises when it goes too far - Fowler specified that it could be said that it's terrible when half of the methods are delegators. |

 

There is also an excellent academic paper accompanying the Github repo, that attempts to survey and classify all code smells: "[Code Smells: A Comprehensive Online Catalog and Taxonomy](https://madeyski.e-informatyka.pl/download/JerzykMadeyski23.pdf)" by Marcel Jerzyk and Lech Madeyski.

Boolean Flags are so popular they may need additional reference sources to wipe out: [Are Boolean Flags on Methods a Code Smell?](https://ardalis.com/are-boolean-flags-on-methods-a-code-smell/) [Clean code: The curse of a boolean parameter](https://medium.com/@amlcurran/clean-code-the-curse-of-a-boolean-parameter-c237a830b7a3)

