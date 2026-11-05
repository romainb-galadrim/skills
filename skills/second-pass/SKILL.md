---
name: second-pass
description: Second pass on the changes.
disable-model-invocation: false
---

Do a second pass on the changes.
If the user didn't send a plan or specify the changes, assume it's the uncommitted changes, or the branch against its parent branch.

Examples of things you should do:
- simplify
- reuse
- refactor
- deduplicate
- improve naming
- remove no longer used code
- make the code more readable
- follow codebase conventions
- apply best practices

In other words, use your taste to improve code quality and readability before we consider it done.
Better code typically results in fewer lines.

Make your improvements in 2 steps:
1. High level (architecture, files organization, code organization, abstractions, etc.)
2. Low level (function bodies, expressions, control flow, etc.)

This is not a correctness or security review; don't focus on logic at the expense of everything else.

If there is nothing to improve, that's fine. Don't make artificial changes just for the sake of it.
(In particular, don't just create one-off helpers and call that an improvement.)

Don't forget any part of the diff.

After you finished, check the results of your changes and ask yourself for each change: "If I was presented with the two versions of the code (before and after the change), which one would I prefer?". Keep the best version.
Don't be afraid to revert if you realize that a change was not an improvement when looking at the result.

Do this process over and over again until you think nothing else can be improved.
