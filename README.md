# Uncommon HTML Bug: Incorrect querySelectorAll Usage

This repository demonstrates an uncommon bug related to the use of `document.querySelectorAll` in HTML.

The bug arises from an attempt to select all elements with a tag name that also happens to be an attribute name ('class' in this case). This leads to unexpected behavior and incorrect selection of elements.

The `bug.html` file contains the buggy code. The `bugSolution.html` file shows the corrected version.

## Bug Description:

The `querySelectorAll` method is used incorrectly to select elements. It's supposed to select elements based on a CSS selector, but using a tag name that doubles as an attribute name will not produce the expected result.  It selects elements with the attribute, not the tag.

## Solution:

The solution involves using a proper CSS selector to target elements based on either their tag name or other attributes. For example, to select all `<div>` elements, use `querySelectorAll('div')`. 