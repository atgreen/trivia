# EGCL support

The `egcl` branch uses Trivia's portable implementation. SBCL-only optimizations remain disabled. Install the EGCL forks of its dependencies, including introspect-environment and named-readtables.

`egcl-tests.lisp` loads this checkout and verifies list, cons, vector and nonmatching patterns. Run with dependencies registered in ASDF: `egcl --no-init --load egcl-tests.lisp`.

These are focused semantic checks, not the complete upstream suite. Optimization and exhaustiveness diagnostics are limited by EGCL's type introspection.
