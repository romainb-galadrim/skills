---
name: simplification-review
description: Ask the agent to look for opportunities to simpilfy and improve the changes. Triggered by the user, never by the agent.
disable-model-invocation: true
---

Look at the changes, look for these:
- things to simplify (big or small)
- unnecessary complicated code for things that are not worth it, or impossible edgecases
- badly written code not reusing existing code
- archictecture improvements (files or code to split, merge, or move in a better place in the file tree)
- technical debt
- code no longer used that can be cleaned up
- names that don't make sense anymore
- code now used only once that could be inlined

This is NOT a traditional code review, don't focus on edge cases or correctness problems, there is another skill for that.
Instead, use your taste to judge the code and suggest improvements.
Don't typecheck or lint, assume it passes.
Don't edit yet.