# CSS ::before/::after content property unexpected rendering bug

This repository demonstrates a subtle bug related to the use of the `content` property within CSS `::before` and `::after` pseudo-elements.  The issue arises when providing complex or unexpected values to the `content` property, potentially leading to unexpected rendering or browser errors.

The `bug.css` file showcases the problematic code, while `solution.css` provides a corrected version.

## Bug Description

Using excessively complex strings, especially those containing certain Unicode characters or dynamically generated content, within the `content` property can result in rendering inconsistencies or errors.  The problem isn't always apparent and might only manifest in specific browsers or contexts.

## Reproduction Steps

1. Open `bug.html` in a web browser.
2. Observe the unexpected rendering or potential error in the output.

## Solution

The solution involves carefully sanitizing and simplifying the values provided to the `content` property, ensuring they are well-formed and compatible across various browsers.