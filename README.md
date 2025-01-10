# MongoDB $inc operator error: Invalid increment value
This example demonstrates an error that can occur when using the `$inc` operator in MongoDB update operations. The `$inc` operator is used to increment a numerical field by a specified value. However, if an invalid value (such as a string) is provided, the operation will fail.

## Bug
The bug lies in the incorrect usage of the `$inc` operator.  The code attempts to increment the `count` field by the string 'abc', which is not a valid numerical value.

## Solution
The solution is to ensure that the value provided to the `$inc` operator is a valid number. The following corrected code demonstrates this:
