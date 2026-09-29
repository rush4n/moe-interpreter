# Interpreter 001 — Arithmetic

## What I Learned

Concrete syntax is what the programmer writes; the AST is the structure the rest of the implementation actually works with. Parentheses and precedence matter while parsing, but once parsing is finished, that information has already been turned into the shape of the tree. The interpreter should not need to reason about precedence again.

The interpreter is an executable definition of the language's semantics. Each AST variant gets one case describing its meaning. Arithmetic is compositional because the result of a larger expression is obtained from the results of its immediate subexpressions.

The recursive structure is doing two jobs here. It defines which expressions exist, and it gives the interpreter its recursion scheme. That connection between the syntax definition and the semantic function is the main reason AST-based interpreters stay manageable as a language grows.
