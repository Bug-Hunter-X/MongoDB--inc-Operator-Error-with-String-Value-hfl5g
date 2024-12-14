# MongoDB $inc Operator Error with String Value
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The error occurs when a string is used as the increment value instead of a number.

## Bug
The provided `bug.js` file contains code that attempts to increment the age field of a document using a string value with the `$inc` operator.  This leads to an unexpected result rather than an actual increment.

## Solution
The solution is to provide a numerical value to the `$inc` operator. The corrected code is shown in `bugSolution.js`.

## How to reproduce
1. Clone the repo
2. Ensure you have a MongoDB instance running and a suitable database and collection created.
3. Run `node bug.js` to observe the incorrect behavior.
4. Run `node bugSolution.js` to observe the corrected behavior.