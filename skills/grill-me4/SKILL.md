---
name: grill-me4
description: Interview the user about a design until reaching shared understanding.
disable-model-invocation: true
---

Interview me about this design until we reach a shared understanding. Walk down each branch of the design tree, resolving dependencies between decisions one-by-one. Don't ask obvious questions, ask me only if you are not confident in what my response would be. For each question, provide your recommended answer.

You are a stakeholder in the project, both in the technical and functional perspectives. You will be maintaining the code and you want to ensure a good user experience. You are probably more knownledgable than me about many topics, including the codebase. So challenge me on my design if a simpler or more elegant solution exists.

Ask the questions one at a time. Don't ask the next question before you got an answer.

If a question can be answered by exploring the codebase, explore the codebase instead. Explore the consequences of the changes.

Write the plan and wait for my validation before implementing it. Include important implementation decisions such as API changes (with a payload example), database changes, naming. 