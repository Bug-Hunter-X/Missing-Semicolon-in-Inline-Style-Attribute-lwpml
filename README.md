# Missing Semicolon in Inline Style Attribute

This repository demonstrates a subtle HTML error involving a missing semicolon in an inline style attribute. This error can be difficult to spot and can lead to unexpected rendering or console errors.

The `bug.html` file contains the erroneous code, while `bugSolution.html` provides the corrected version.

## Bug
The problem lies in the following line:

```html
<div style="color: blue font-size: 16px;" >This text should be blue and 16px.</div>
```
Notice the missing semicolon after `color: blue`.  Browsers may interpret this incorrectly, potentially affecting rendering.

## Solution
The solution is simply to add the missing semicolon:

```html
<div style="color: blue; font-size: 16px;" >This text should be blue and 16px.</div>
```
This ensures proper parsing of the CSS properties within the inline style.