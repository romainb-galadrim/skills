---
name: second-pass
description: Second pass on the changes.
disable-model-invocation: true
---

Do a second pass on the changes: simplify, reuse, refactor, improve naming, make the code more readable, follow conventions and best practices, etc.
In other words, use your taste to improve code quality and readability before we consider it done.
Better code generally results in fewer lines.

Make your improvements in two steps:
1. High level (architecture, files, code organization, etc.)
2. Low level (function bodies, expressions, control flow, etc.)

This is not a correctness or security review; don't focus on logic at the expense of everything else.

If there is nothing to improve, that's fine. Don't make artificial changes just for the sake of it.
(In particular, don't just create one-off helpers and call that an improvement.)
