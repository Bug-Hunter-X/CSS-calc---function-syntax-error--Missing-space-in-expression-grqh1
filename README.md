# CSS calc() Function Syntax Error: Missing Space

This repository demonstrates a subtle but frustrating error that can occur when using the `calc()` function in CSS.  The issue arises from a missing space between the units and the operator inside the `calc()` expression.

## Problem

The following CSS code snippet is intended to set the width of an element to 10 pixels less than its container's width:

```css
.element {
  width: calc(100%-10px);
}
```

However, this code produces a syntax error because there is no space between `100%` and the minus sign (`-`). The correct syntax requires a space between the units and operators within the `calc()` expression.

## Solution

To fix the error, add spaces around the operators within the `calc()` expression:

```css
.element {
  width: calc(100% - 10px);
}
```

This corrected version will correctly calculate the width of the `.element`.

This demonstrates the importance of paying close attention to the syntax when using the CSS `calc()` function to prevent unexpected behavior and errors.