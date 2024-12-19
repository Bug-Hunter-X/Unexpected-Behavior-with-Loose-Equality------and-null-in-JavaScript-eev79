# JavaScript Loose Equality Bug

This repository demonstrates a common JavaScript bug related to loose equality (`==`) when comparing values to `null`. Loose equality can lead to unexpected behavior, especially when dealing with `null` and `0`.

## Bug Description
The `foo` function uses loose equality (`==`) to check for `null` values.  This can cause unexpected results because `0 == null` evaluates to `true`.

## Solution
The solution uses strict equality (`===`) to correctly compare against `null`.  Strict equality checks for both value and type, making it more reliable and preventing unexpected behavior.

## How to Reproduce
1. Clone the repository.
2. Run `bug.js` using Node.js or a browser's console. Observe the unexpected output.
3. Run `bugSolution.js`. Note that this version produces the expected behavior.