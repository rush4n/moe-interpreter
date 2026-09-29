# Homework 002 — Structural Recursion

## What I Learned

The definition of a recursive datatype already tells me the basic shape of functions over it. Since a `Tree` is either a leaf or a node containing two more trees, a structurally recursive function needs the same two cases and recursive calls for the two subtrees. The datatype and the function are following the same induction principle.

An accumulator is useful when the answer at the current value depends on the path used to reach it. For the summary-leaf check, the accumulator is not part of the tree itself; it is context passed downward from the root. The public function starts that context, while the helper maintains it during recursion.

The list exercise was also a concrete example of universal quantification. Checking that every tree satisfies a property becomes recursion with conjunction. Returning true for the empty list is not a special trick—it is the usual vacuous-truth case for “every element satisfies the predicate.”
