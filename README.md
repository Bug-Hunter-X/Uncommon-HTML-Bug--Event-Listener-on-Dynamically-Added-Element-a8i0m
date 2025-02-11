# Uncommon HTML Bug: Event Listener on Dynamically Added Element

This repository demonstrates a common but easily missed bug when adding event listeners to dynamically created HTML elements using `innerHTML`.

## The Bug

The `bug.html` file contains a simple HTML page with a div element.  JavaScript attempts to add a button to this div using `innerHTML` and assigns an `onclick` event handler.  This approach is problematic because the event listener is not properly attached to the dynamically created element.

## The Solution

The `bugSolution.html` file demonstrates the corrected approach. Instead of using `innerHTML`, it uses `createElement` to create the button element and `addEventListener` to correctly attach the event listener.