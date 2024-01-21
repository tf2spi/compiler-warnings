# compiler-warnings
Nice compiler warnings categorized by potential bug severity

## Compilers

Different directories in this repo represent the flags for
different compilers, like ``gcc``, ``clang``, ``cl``, etc.


## Severity

Inside each different compiler is a few text files describing
the flags that fall under a certain severity.

* ``corruption.txt``: These warnings deal with issues that have
  a high probability of causing memory corruption, a crash, or
  a pointer leak.

* ``suspect.txt``: These don't suggest immediate error but the pattern
  is strange enough to likely not be what is desired from the programmer.

* ``pedantic.txt``: Compiler will likely do what you want, but just
  to be safe, enforce rules that technically cause undesired behavior.
  All "unused" warnings go here as well.


