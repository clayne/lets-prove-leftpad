# Lean 4 leftpad

This is a port (but not literal) of the `leftpad` function and correctness proofs
from the now deprecated Lean version 3 to the [Lean 4](https://lean-lang.org/)
theorem prover.


## About Lean 4

Lean 4 is a Dependently-Typed Programming Language designed for verified
programming, featuring efficient run-time system (with multithreading), flexible
macro system (with syntactic extensions and elaborator reflection) and some
advanced type system elements (quotient types, mutual and nested inductive
types, etc.). Thanks to strict separation of total and non-total functions,
as well as great interactive development support via VS Code and Emacs plugins,
Lean 4 also excels as a Proof Assistant for formalizing mathematics as evidenced
by the [Mathlib](https://github.com/leanprover-community/mathlib4) project.


## About the Code

The first part is a literal translation of the `leftpad` function from the
Lean 3 [code](../leanprover/leftpad.lean), it's defined in terms of lists of
arbitrary elements (not necessarily characters).

The second part in the `Strings` namespace defines another version of `leftpad`
operating on `String`s (which are internally UTF8 strings in Lean 4).


## About me

I'm Alex Chichigin ([Github](https://github.com/gabriel-fallen/),
[blog](https://dev.to/gabrielfallen)) a formal methods enthusiast. :)

The proofs for `Strings` version were contributed by
[Сухарик](https://github.com/suhr).
