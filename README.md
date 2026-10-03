# Programming Languages and Interpreters

This repository tracks my CS6520 coursework [and beyond ;)]

## Homeworks

- [`homeworks/001/basics.rhm`](homeworks/001/basics.rhm): Typed functions, strings, algebraic datatypes, and pattern matching.
- [`homeworks/002/basics_cntd.rhm`](homeworks/002/basics_cntd.rhm): Structural recursion over trees and lists, including an accumulator for path-dependent state.
- [`homeworks/003/functions.rhm`](homeworks/003/functions.rhm): Extends the first-order function interpreter with `max`, zero-or-more arguments, call-by-value substitution, and arity checking.

## Interpreters

- [`interpreters/001/interpreter.rhm`](interpreters/001/interpreter.rhm): An arithmetic parser and interpreter built around an explicit AST.
- [`interpreters/002/interpreter.rhm`](interpreters/002/interpreter.rhm): Adds identifiers and first-order functions using definition lookup and substitution.
- [`interpreters/003/interpreter.rhm`](interpreters/003/interpreter.rhm): Replaces substitution for local variables with an explicit environment and adds lexically scoped `let` bindings.
- [`interpreters/004/interpreter.rhm`](interpreters/004/interpreter.rhm): Adds closures, boxes, sequencing, and an explicit store that threads state through evaluation.
