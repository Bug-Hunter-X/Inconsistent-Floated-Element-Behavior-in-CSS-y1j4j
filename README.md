# Inconsistent Floated Element Behavior in CSS

This repository demonstrates a common issue with floated elements in CSS where the behavior can be inconsistent across different browsers.  When the combined width of floated elements exceeds the width of their parent container, unexpected wrapping or collapsing can occur.  This is due to how browsers handle the interaction between floated elements and the normal document flow.  The provided solution shows a method to mitigate this issue.

## Bug Report

The `bug.css` file contains the CSS code that exhibits this inconsistent behavior.  The problem is evident when the total width of the divs exceeds their container's width.  Different browsers may render this differently, leading to unexpected layout results.

## Solution

The `bugSolution.css` file provides a solution using `clearfix` (or other appropriate methods).  This addresses the issue by clearing the floats and ensuring the parent container properly contains the floated elements.  The solution uses a CSS class to ensure it can be easily applied in various contexts.