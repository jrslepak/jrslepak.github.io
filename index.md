---
layout: home
---

I am a PhD candidate at
[Northeastern University's Programming Research Lab](http://prl.ccs.neu.edu),
interested in the design of programming languages,
especially high-level languages for parallel programming.
The main topic areas that have fed into my research are:
* formal semantics and type systems
* compilation and optimization
* decision procedures and constraint solving


My thesis research is centered around designing Remora,
an array-oriented programming language in which
implicit, data-driven control flow lifts all operations to work on
arbitrarily high-dimensional arrays,
including functions which expect array arguments to begin with,
like matrix inversion.
In effect, each function call automatically becomes
a loop nest appropriate for the particular function and arguments.
Remora uses a restricted form of dependent types
to track the shapes of arrays produced during execution,
which statically identifies the implicit iteration structure
and ensures compatibility between functions and their arguments.
Functions can be parameterized over
individual dimensions and shapes (sequences of dimensions),
allowing operations like summing along an array's major axis.
The best detailed overview of the project is a
[journal manuscript](https://arxiv.org/abs/1907.00509)
currently under review.

Current work on Remora is focused on type inference,
to automatically instantiate dependently-typed functions at call sites
and identify their dimension and shape arguments when they are defined.
