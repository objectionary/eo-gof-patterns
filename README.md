# EO Design Patterns

## Introduction
The activity of finding the right design pattern is one of the most difficult task in software development and developers, who have eagerly adopted design patterns over the past years, needed to understand not only the various design patterns available but the software systems as well and then be able to maintain these software systems, even in cases where documentation and/or design models are missing or of a poor quality. In most cases only the source code as the basic form of documentation is available.
## Goal and Motivation
To analyse design patterns by implementing some popular design patterns in EO. This is to help better assess the EO programming language and suggest alternatives of design patterns in EO that could replace such patterns which are not supported in the language.
This repository contains descriptions and EO implementation of some popular software design patterns.

## Implemented patterns
Description of the design patterns analysis is available [here](https://github.com/HSE-Eolang/eodesignpatterns/tree/main/tex).
The following design patterns are implemented:
- [Abstract Factory](https://github.com/HSE-Eolang/eodesignpatterns/blob/main/eo/AbstractFabric.eo)
- [Adapter](https://github.com/HSE-Eolang/eodesignpatterns/blob/main/eo/Adapter.eo)
- [Bridge](https://github.com/HSE-Eolang/eodesignpatterns/blob/main/eo/Bridge.eo)
- [ChainOfResponsibility](https://github.com/HSE-Eolang/eodesignpatterns/blob/main/eo/ChainOfResponsibility.eo)
- [Command](https://github.com/HSE-Eolang/eodesignpatterns/blob/main/eo/Command.eo)
- [Composite](https://github.com/HSE-Eolang/eodesignpatterns/blob/main/eo/Composite.eo)
- [Decorator](https://github.com/HSE-Eolang/eodesignpatterns/blob/main/eo/Decorator.eo)
- [Mediator](https://github.com/HSE-Eolang/eodesignpatterns/blob/main/eo/Mediator.eo)
- [Null object](https://github.com/HSE-Eolang/eodesignpatterns/blob/main/eo/NullObject.eo)

## Conclusion
It is possible to conclude that (1) EO is principally applicable to all the considered patterns; (2) For some patterns, EO is able to give a fairly concise and intuitively clear code, since the language combines the features of Functional Programming and OOP.

Also, EO has no local variables or any kind of stack-lifetime storage. Instead, any name refers to an object (stored in heap) that may be accessed through the scope of any other object via the dot-notation mechanism. Even anonymous objects may allow programmers to access its local scope (including parent and decoration hierarchies) freely. In addition, EO has no access modification instruments. This makes closures technique almost similar to the partial application mechanism. Moreover, the publicity of any attribute of any object makes encapsulation impossible in the language. This differentiates EO from functional programming languages and, also, from object-oriented languages. Absence of instruments of access modification (or simulation of it) may be a severe violation of object-oriented principle of encapsulation, which may lead to insecure environments breaking business logic of problem domains.
