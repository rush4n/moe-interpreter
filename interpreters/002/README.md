# Interpreter 002 — First-Order Functions

## What I Learned

Adding functions introduced the distinction between binding an identifier and using one. A function parameter binds matching identifiers in its body. If an identifier reaches the interpreter without such a binding, it is free, so evaluation cannot assign it a value.

Function application is modeled directly with substitution. The interpreter evaluates the argument, turns the resulting number back into an expression, replaces the parameter in the body, and then interprets the new body. This is a simple semantic model of call-by-value, even though a production interpreter would usually use an environment instead of repeatedly rewriting syntax.

The language is first-order because function names are resolved in a separate collection of definitions. Functions are not part of the value space, so they cannot be passed around like integers.

I also saw the difference between syntax errors and semantic errors more clearly. A free variable or an unknown function call can be parsed into a valid AST, but evaluation still fails because the program has no meaning under the rules currently defined by the interpreter.
