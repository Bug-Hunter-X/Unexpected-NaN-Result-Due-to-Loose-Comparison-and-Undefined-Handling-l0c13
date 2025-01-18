# Unexpected NaN Result Due to Loose Comparison and Undefined Handling

This repository demonstrates a common JavaScript error related to loose comparison and the handling of `null` and `undefined` values.  The `bug.js` file contains code that attempts to gracefully handle `null` inputs but fails to account for `undefined`, resulting in `NaN` (Not a Number).

The `bugSolution.js` file provides a corrected version, showcasing best practices for handling these edge cases.

## How to Reproduce

1. Clone this repository.
2. Open `bug.js` and observe the unexpected `NaN` output when passing `undefined` as an argument.
3. Compare it to the corrected output in `bugSolution.js`.

## Lesson Learned

It's important to explicitly check for both `null` and `undefined` in JavaScript to avoid unexpected behavior.  Using strict equality (`===`) for comparison is also highly recommended for clarity and to avoid type coercion issues.