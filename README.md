# CSS Specificity Issue: Unexpected Inheritance Behavior

This repository demonstrates a subtle issue related to CSS specificity and inheritance. The problem arises when trying to style a paragraph element (`<p>`) nested within a `div` element, where the styles defined for the parent (`div`) are not inherited correctly.

## Problem Description

When a paragraph element is styled directly (`div p`) and also indirectly through the parent (`div`), the direct style appears to take precedence even if the expectation is to inherit styles from the parent and only override when a specific style is applied to the `div p`.

## Solution

The provided solution demonstrates that using the `!important` flag is not always required to style based on CSS specificity. Instead, focus on creating specific CSS selectors that have the intended precedence. Using `!important` could lead to maintenance problems and difficult-to-debug issues.