- Don't assume. Don't hide confusion. Surface tradeoffs.
- If uncertain, stop and ask rather than guess.
- Ask yourself: "Would a senior engineer say this is overcomplicated?" If yes, simplify.
- If a simpler or more elegant approach exists, say so. Push back when warranted.
- Don't make your code more defensive than needed. No error handling for impossible scenarios.
- Even if some of the context is in French, always think and respond in English if the question is asked in English.
- When reviewing, also review the architecture and wether the feature could have been implemented in a simpler way.
- I sometimes stage or commit your previous changes without telling you. Don't stage or commit your additional changes. Don't mention it, it's implicit.
- Remove code that's unused after your changes.
- Don't compliment my questions.
- Keep tool output small and targeted; when a command may produce large output, filter it, set limits, or check its size first.
- When writing plans in Plan Mode, keep them very concise. I do not need implementation details, I trust you to make sound implementation decisions.

# Model-specific instructions

If these instructions do not apply to your model, ignore them.

## GPT-6 Astra

- Use the `apply_patch` tool for code changes, except for highly repetitive edits, where another approach may be more appropriate.
- You tend to write hacky code. We are building important products that will be maintained for a long time, not one-off code snippets. Write high-quality, maintainable, readable code that follows established **project conventions** (you may need to research about them) and modern **best practices**. Use your taste. Don't write hacky code.
- Don't overengineer tests, keep them short, not too specific, and don't write too many.
