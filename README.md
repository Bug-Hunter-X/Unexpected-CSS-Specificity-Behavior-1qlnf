# Unexpected CSS Specificity Behavior

This repository demonstrates a subtle CSS specificity issue where a nested selector unexpectedly overrides an ancestor selector. The bug arises from the interplay of inheritance and specificity.

## Bug Report

The primary issue lies in how the `.child` element's style is determined.  The specificity of the nested selector `#parent .child` outweighs that of the `.child` selector, resulting in unintended styling.

## Solution

The solution involves understanding CSS specificity rules and possibly adjusting the selector order or using `!important` (though this is generally discouraged). The solution file provides a corrected CSS rule set.