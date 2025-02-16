# Hidden HTML element not reappearing

This repository demonstrates an uncommon bug in HTML where an element, after having its display set to `none`, does not reappear when the display is subsequently set to `block`.  The issue is compounded by clearing the element's innerHTML.

## Bug Description
The bug occurs when we first clear the content of a div element using `innerHTML = "";`, then set its display style to `none`, and finally attempt to make it visible again by setting the display style to `block`. The div remains hidden even after changing the display property to 'block'.

## How to Reproduce
1. Open `bug.html` in a web browser.
2. Click the button.
3. Observe that the div with the id "myDiv" remains hidden even though its display is set to 'block'.

## Solution
The solution involves removing the `innerHTML` assignment before changing the `display` property or using a different approach to show and hide content. Refer to `bugSolution.html` for a working example.