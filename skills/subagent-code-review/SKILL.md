---
name: subagent-code-review
description: Ask a subagent for a code review and address the issues
disable-model-invocation: true
---

If the changes are unstaged, stage them, so we can easily see the new changes (that will be left unstaged).
Create a subagent with the `second-pass` skill, for the changes/PR.
Give it a very minimal prompt, with just the skill and what changes.
Once it's done, check the changes and make sure you agree with them. You can revert/modify them otherwise.
Stage the changes.

Then, create another subagent with the `code-review` skill, to review the changes/PR.
Give it a very minimal prompt like "Use the `code-review` skill to review the changes", so it's unbiased.
Just add these instructions:
- For conventions, don't just review compliance with CLAUDE.md or AGENTS.md files, but also and more importantly, repository conventions and modern best practices.
- There are no upper limits for the number of findings (if the skill specifies some, ignore them).
- Use tools at your disposal to verify your claims.
- Do not run checks that will take a long time such as compilation.

Then, decide which problems are correct and worth addressing.
Don't overengineer, the code shouldn't get bloated for unrealistic edge cases.
Discuss with the agent until you come to an agreement.
Then implement the fixes.
You can ask me questions if some fixes require a decision or walking back on a previous decision.
Read the new changes you made, and for each one, ask yourself if it's worth it. If not, revert it.
Report the fixes and the rejections (with the numbers, so I can reference them).
If there are any important changes I should be aware of, mention them in a section below.
