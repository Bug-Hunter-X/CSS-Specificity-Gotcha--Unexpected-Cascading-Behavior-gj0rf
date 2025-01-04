# CSS Specificity Gotcha: Unexpected Cascading Behavior

This repository demonstrates a subtle issue related to CSS selector specificity and the cascading order of styles.  It highlights a scenario where a seemingly less specific selector unexpectedly overrides a more specific selector due to how CSS specificity is calculated. The example shows how the unexpected cascading can lead to unexpected styling outcomes.

## Bug Description
The bug is demonstrated by the fact that the styling of a `p` element within a `div` is influenced by a selector targeting `p` even when there is a more specific selector (`div p`).

## Solution
The solution involves a deeper understanding of CSS specificity and carefully crafting selectors to ensure the desired styling behavior.  This might involve using `!important` (generally discouraged) or restructuring the HTML to provide clearer separation of concerns.

## How to Reproduce
Clone this repository and open `bug.html` in your browser.  Note the unexpected styling.  Then, compare that to `bugSolution.html` to observe the corrected output.