# Programming Languages Concepts

This repository tracks my CS6520 coursework (and beyond ;)

## Programming-Language Theory

- **Concrete and abstract syntax:** Surface notation is parsed into an inductively defined abstract syntax tree. Precedence and grouping belong to parsing; evaluation operates on the resulting structure.
- **Syntax–semantics separation:** Syntax determines which programs can be represented, while semantics assigns meaning to those representations. An interpreter is an executable semantic function over the AST.
- **Compositional interpretation:** The meaning of a compound expression is defined recursively in terms of the meanings of its subexpressions.
- **Binding and scope:** Identifiers are classified by their binding occurrences and uses. An unbound identifier is a free variable and therefore produces a semantic error in the current language.
- **Substitution semantics:** Function application can be modeled by replacing formal parameters in a function body with argument values while respecting the recursive structure of the syntax.
- **Evaluation strategy:** The interpreters use call-by-value semantics. Argument expressions are evaluated before substitution, so only resulting numeric values enter a function body.
- **First-order functions:** Function definitions live in a separate global collection and are referenced by name; functions are not yet values that can be passed or returned.
- **Arity as a dynamic invariant:** Multi-argument application traverses formal parameters and actual arguments in parallel and rejects mismatched list lengths.
- **Inductively defined data:** ASTs, lists, and trees are recursive datatypes. Their eliminators follow the datatype's structure, which provides the implementation template for parsers, interpreters, substitution, and analyses.
- **Language extensibility:** Adding a construct requires coordinated changes to the grammar, AST, parser, semantic function, substitution traversal, and tests. This exposes the coupling between a language's representation and its metatheoretic operations.
- **Programs as data:** Once syntax has an explicit representation, programs can be constructed, transformed, inspected, and interpreted like other recursive data.

## Coursework

- `homeworks/001`: functions, strings, conditionals, datatypes, variants, and pattern matching
- `homeworks/002`: binary trees, structural recursion, lists, helpers, and accumulators
- `homeworks/003`: language extensions, functions, substitution, multiple arguments, and arity checking

## Interpreter Progress

- `interpreters/001`: arithmetic AST, parser, and interpreter
- `interpreters/002`: identifiers, first-order functions, definition lookup, substitution, and call-by-value evaluation
