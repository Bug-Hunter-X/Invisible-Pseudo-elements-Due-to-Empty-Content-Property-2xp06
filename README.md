# Invisible Pseudo-elements in CSS

This repository demonstrates a common yet subtle error in CSS involving pseudo-elements (::before and ::after) and their `content` property.  The issue arises when the `content` property is set to an empty string, resulting in an invisible pseudo-element even if other styles are applied.

## Bug

The `bug.css` file contains the erroneous CSS. The pseudo-element is technically applied, but it remains invisible due to the empty string in `content`. 

## Solution

The `bugSolution.css` file shows the corrected CSS.  Simply replacing the empty string with an actual value (e.g., a non-breaking space `&nbsp;`, a string, or an image URL) solves the problem.