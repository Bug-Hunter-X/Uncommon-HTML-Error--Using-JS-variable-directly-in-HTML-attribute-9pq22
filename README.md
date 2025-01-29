# Uncommon HTML Error: Using JS Variable Directly in HTML Attribute

This repository demonstrates a common error in HTML: attempting to use a JavaScript variable directly within an HTML attribute.  This often results in a runtime error because JavaScript variables are not available in the HTML rendering context.

## Problem
The problem lies in directly referencing a JavaScript variable (e.g., `myVar`) inside an HTML attribute like `onclick` before the script executing and assigning a value to that variable has a chance to run.  HTML parsing happens first, and the value of `myVar` will be undefined during this initial stage.

## Solution
The solution involves using event listeners in JavaScript after the HTML element has been rendered.

## How to run the code
1. Clone this repository.
2. Open `bug.html` in your browser to see the error. 
3. Open `bugSolution.html` to see the correct way to resolve this issue.

## License
MIT