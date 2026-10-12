---
name: simplification-review
description: Identify which parts of the changes or plan we could simplify.
disable-model-invocation: true
---

Look at the changes or plan and identify which parts of the feature offer the least value relative to the complexity they add.
If the user didn't send a plan or specify the changes, assume it's the uncommited changes, or the branch against its parent branch.

Consider both perspectives:
- As a user, how useful and intuitive is this behavior?
- As a maintainer, how annoying is the code to read and maintain?

Recommend which parts of the changes or plan you would drop to deliver the most value **over the long term**. The tradeoff is that keeping this complexity to add value now might slow down our ability to add value later.
