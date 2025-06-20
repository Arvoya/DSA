# Functional Programming

> *Functional Programming (FP)* is a programming paradigm based on functions,
which are the only building blocks for your code. Using FP improves your code's
modularity and helps you write more understandable, testable, and easy-to-
maintain code while avoiding bugs; it's a win all around.

There are many varied opinions between FP and *object-oriented programming
(OOP)*, which is better and why, and how one is better in the *real world* than
the other. Personally, I lean towards FP, but I also think there's more for me to
learn.

This book seems to lean into it, so I'll take notes that reflect the books/
authors interest.

## Why Use Functional Programming?

* Understandable
* Maintainable
* Testable
* Modular
* Reusable

> Of course, OOP can do all of these things as well. No one is ever going to say
that FP is a silver bullet that solves all your software development problems. I
always suggest taking the middle road; a well-thought-out, balanced mix is
usually the best solution.

## JavaScript as a Functional Language

> For the purposes of this book, we'll consider language to be functional if (and
only if) it supports common FP features.

### Functions as First-Class Objects

> means you can do anything them that you'd be able to do with other objects.

* Store functions in variables
* Pass functions as arguments
* Return a functions as a result from another function

### Declarative-Style Programming

> FP works in higher-level, *declarative* style instead of the imperative style
used in procedural, "common" programming.

```js
.filter()
.find()
.some()
.map()
.reduce()
```

### Higher-Order Functions

> Functions that receive other functions as arguments are that return functions
as results are called *higher-order functions*.
