# Unexpected Behavior of calc() within ::before Pseudo-element

This repository demonstrates an uncommon issue related to using the `calc()` function in CSS within a `::before` pseudo-element. The problem arises when the parent element's width isn't explicitly defined, causing unexpected behavior in the `calc()` function.

## Bug Description
The `calc()` function, intended to calculate the width dynamically, fails to function as expected if the parent element's width is determined implicitly. This is particularly noticeable when used with pseudo-elements like `::before`.

## Solution
Explicitly define the width of the parent element to resolve the issue. This provides a concrete value for `100%` within the `calc()` function, ensuring accurate calculations.

## Files:
- `bug.css`: Contains the CSS code exhibiting the unexpected behavior.
- `bugSolution.css`: Provides the corrected CSS code with an explicit parent width.