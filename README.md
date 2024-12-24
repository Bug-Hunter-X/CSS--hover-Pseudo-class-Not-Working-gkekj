# CSS :hover Pseudo-class Not Working

This repository demonstrates a common CSS issue where the `:hover` pseudo-class does not function as expected.  The problem arises when an element with a higher z-index or an element that captures mouse events overlays the element intended to trigger the hover effect.  The solution involves adjusting z-index values, pointer-events, or addressing any event capturing issues to ensure the hover event propagates correctly.

## Bug
The provided CSS code attempts to change the background color of a div element when hovered.  However, due to an overlapping element, the hover effect is not triggered.  See `bug.css` for the faulty code and `index.html` for the HTML structure.

## Solution
The solution involves addressing the overlapping element by ensuring that it doesn't block the hover event.  See `solution.css` for the corrected code.  The HTML structure remains unchanged, demonstrating the solution works with the original HTML setup.

## Reproduction Steps
1. Clone the repository.
2. Open `index.html` in your browser.
3. Hover over the blue square. You will notice the hover effect is blocked in `bug.css` but works as expected in `solution.css`.