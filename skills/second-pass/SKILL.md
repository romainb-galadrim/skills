---
name: second-pass
description: Second pass on the code. Triggered by the user, never by the agent.
disable-model-invocation: true
---

Do a second pass on the code. See if there is anything you can simplify, reuse, refactor, name better, make more readable, use less lines, etc. In other words, use your taste to improve code quality and readability before we consider it done. This is not a correctness or security review, don't focus on the logic to the expense of the rest. If there is nothing to improve, it's fine, don't make artificial changes just for the sake of it.
