# MongoDB $inc Operator Error
This example demonstrates an error that can occur when using the `$inc` operator in MongoDB if you provide a string instead of a number.
The `$inc` operator is used to increment a numerical field by a specified value. Providing a string will cause an error.
## Bug
The bug is in the `updateOne` operation where we attempt to increment the `count` field by '1' (a string) instead of 1 (a number).
## Solution
The solution is simple: Use a number instead of a string when incrementing the field value using the `$inc` operator.
