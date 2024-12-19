# CSS Float and Width Issue in Older Browsers

This repository demonstrates a common CSS issue related to floating elements and their width when the parent container doesn't have an explicitly set width.  Some older browsers may interpret `width: 50%;` unexpectedly in this scenario. 

The `bug.css` file contains the problematic CSS, while `bugSolution.css` offers a solution to ensure consistent rendering across different browsers.

## Problem

The issue lies in the use of `float: left;` and `width: 50%;` on a `div` element when its parent container's width isn't defined. In some browsers, this can lead to the `div` not occupying the expected 50% of the available space, possibly resulting in unexpected layout.

## Solution

The solution involves ensuring the parent container has a defined width (e.g., `width: 100%;` or a fixed pixel width) or using alternative layout techniques like flexbox or grid.