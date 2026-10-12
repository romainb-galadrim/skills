---
name: simplification-review2
description: Identify which parts of the changes or plan we could simplify.
disable-model-invocation: true
---

Look at the changes or plan and identify which parts of the feature offer the least value relative to the complexity they add.

Consider both perspectives:
- As a user, how useful is this behavior?
- As a maintainer, how annoying is the code to read and maintain?

Recommend which parts of the changes or plan you would drop to deliver the most value **over the long term**. The tradeoff is that keeping this complexity to add value now might slow down our ability to add value later.
