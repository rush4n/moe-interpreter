# Homework 003 — Extending a First-Order Language

## What I Learned

Adding an operator is a change to the language, not just a new branch in the parser. The construct needs a representation in the AST, a parsing rule, an interpretation rule, and support in every operation that traverses expressions, such as substitution. Missing one of those places means the language extension is incomplete.

Changing functions from one argument to any number of arguments turned parameters and arguments into lists. The important part is that the two lists have to be consumed together. If one ends before the other, the call has the wrong arity.

The interpreter uses substitution semantics for function calls: evaluate an argument and replace its parameter in the body. Evaluating first is the call-by-value choice. It matters even when a parameter is unused, because an invalid argument expression must still fail before the function body runs.

These are still first-order functions. A function is found by its name in a separate list of definitions; it is not itself a value that can be passed to or returned from another function.
