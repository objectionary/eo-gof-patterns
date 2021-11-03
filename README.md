<img src="https://www.yegor256.com/images/books/elegant-objects/cactus.svg" height="100px" />

The activity of finding the right design pattern is one of the most difficult task 
in software development and developers, who have eagerly adopted design patterns 
over the past years, needed to understand not only the various design patterns 
available, but the software systems as well and then be able to maintain these s
oftware systems, even in cases where documentation and/or design models are 
missing or of poor quality. In most cases only the source code as the basic 
form of documentation is available.

This repository contains implementation of some popular software design 
patterns in the [EO](https://www.eolang.org) programming language. These patterns 
were implemented with the goal of analyzing design patterns in the 
context of C++ and Java with the intention to help better assess EO and suggest 
alternatives of design patterns in EO that could replace such patterns 
which are not supported in the language.

Description of the design patterns analysis is available [here](https://github.com/HSE-Eolang/eodesignpatterns/tree/tex).
The following design patterns are implemented:

- [Abstract Factory](/src/eo/AbstractFabric.eo)
- [Adapter](/src/eo/Adapter.eo)
- [Bridge](/src/eo/Bridge.eo)
- [ChainOfResponsibility](/src/eo/ChainOfResponsibility.eo)
- [Command](/src/eo/Command.eo)
- [Composite](/src/eo/Composite.eo)
- [Decorator](/src/eo/Decorator.eo)
- [Mediator](/src/eo/Mediator.eo)
- [Null object](/src/eo/NullObject.eo)

## How to Run?

NB: You will need to have the HSE eo compiler installed (built and installed on your computer).

You can include these patterns in EO compiler sandbox folder 
and run with the following commands:

First, compile it:

```bash
mvn compile
```

The, run:

```
./run.sh <name-of-pattern>
```

The `<name-of-pattern>` must be as specified in the code.

## Our Conclusion

It is possible to conclude that (1) EO is principally applicable 
to all the considered patterns; (2) For some patterns, EO 
is able to give a fairly concise and intuitively clear code, 
since the language combines the features of Functional Programming and OOP.

Also, EO has no local variables or any kind of stack-lifetime storage. Instead,
any name refers to an object (stored in heap) that may be accessed through the
scope of any other object via the dot-notation mechanism. Even anonymous objects
may allow programmers to access its local scope (including parent and decoration
hierarchies) freely. In addition, EO has no access modification instruments.
This makes closures technique almost similar to the partial application
mechanism. Moreover, the publicity of any attribute of any object makes
encapsulation impossible in the language. This differentiates EO from functional
programming languages and, also, from object-oriented languages. Absence of
instruments of access modification (or simulation of it) may be a severe
violation of object-oriented principle of encapsulation, which may lead to
insecure environments breaking business logic of problem domains.

This analysis was made by a team of [HSE University](https://www.hse.ru/en/).
