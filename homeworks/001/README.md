# Homework 001 — Functions and Datatypes

## What I Learned

An algebraic datatype gives a precise description of the possible shapes of a value. A `Light` is either a bulb carrying watts and a technology, or a candle carrying its remaining inches. Those are different cases of the same type, not objects that happen to share an interface.

Pattern matching is the other half of defining variants. The constructors introduce values, and `match` lets a function take them apart. Covering every variant also makes it easy to see whether a function is defined over the whole datatype.

The type annotations act like small specifications. They say what kind of input a function accepts and what it must return without saying anything about the implementation. I also got more comfortable building a larger calculation by composing smaller functions instead of writing it as one expression from scratch.
