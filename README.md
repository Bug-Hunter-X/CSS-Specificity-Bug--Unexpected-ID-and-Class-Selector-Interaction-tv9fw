# CSS Specificity Bug: Unexpected ID and Class Selector Interaction

This repository demonstrates a subtle bug in CSS related to selector specificity. The bug arises from an unexpected interaction between ID and class selectors, leading to unintended styling behavior. The `#main.container` selector unintentionally targets elements with both the ID 'main' and the class 'container', even when a more specific rule might be expected to apply.

## Bug Description

The `bug.css` file contains a CSS rule that is too broad in its application. It affects elements which have both the ID 'main' and the class 'container', even if those elements are nested within other elements that have similar classes or IDs, which is not the intended behavior.

## Solution

The `bugSolution.css` file provides a solution that addresses the specificity issue.  We replace the problematic selector with more specific selectors or use the `:not()` pseudo-class to exclude unintended elements.