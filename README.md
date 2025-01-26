# Unexpected String Concatenation in JavaScript
This repository demonstrates a common error in JavaScript related to loose typing and the unexpected concatenation of strings when performing addition.
## Bug Description
JavaScript's dynamic typing system can lead to surprising results when combining numbers and strings using the '+' operator.  Instead of throwing an error, it performs string concatenation.
## Bug Reproduction
The `bug.js` file contains the problematic code.  Run the code to see the unexpected output where numeric addition is expected, but string concatenation occurs.
## Solution
The `bugSolution.js` file shows how to mitigate this issue by explicitly converting the operands to numbers using `parseInt()` or `Number()` before performing the addition operation. This ensures that addition, rather than string concatenation, is carried out as intended.
## Lessons Learned
Always be mindful of JavaScript's type coercion behaviors.  Explicit type checking or conversion can help avoid unexpected results.