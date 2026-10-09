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
- [`interpreters/005/interpreter.rhm`](interpreters/005/interpreter.rhm): Adds immutable records and field lookup. Functional update produces a new record, making the datatype persistent.
- [`interpreters/006/interpreter.rhm`](interpreters/006/interpreter.rhm): Stores record fields in boxes so assignment updates the existing record. Imperative update makes the datatype mutable.
- [`interpreters/007/interpreter.rhm`](interpreters/007/interpreter.rhm): Adds assignable variables by mapping names to store locations instead of directly to values.
- [`interpreters/008/interpreter.rhm`](interpreters/008/interpreter.rhm): Encodes `let`, booleans, and conditionals using only functions and application, with thunks preserving conditional evaluation under call-by-value.
