# Uncommon DOM Manipulation Bug in HTML/JS

This repository demonstrates a subtle bug related to accessing dynamically generated HTML elements before they're fully added to the Document Object Model (DOM).

## Bug Description
The `bug.html` file attempts to modify the `innerHTML` of an element with a dynamically generated ID. However, this is done before the element with that ID exists in the DOM. This leads to a runtime error.

## Solution
The `solution.html` file showcases the corrected approach.  It waits until the element exists in the DOM before attempting to change its content using `setInterval` or a similar approach for asynchronous operations.