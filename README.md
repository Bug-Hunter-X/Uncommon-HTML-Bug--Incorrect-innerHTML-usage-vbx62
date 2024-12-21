# Uncommon HTML Bug: Incorrect innerHTML usage

This repository demonstrates a common, yet subtle bug in HTML related to DOM manipulation using innerHTML.  The bug arises from attempting to access and modify an element that does not exist in the DOM. This can often happen when working with asynchronous operations or dynamically loaded content. 

## Bug Description
The code attempts to set the innerHTML of an element with the ID 'nonExistentElement'. However, this element is not present in the HTML.  This results in a JavaScript error, preventing the rest of the script from executing correctly.

## Solution
The solution involves checking if the element exists before attempting to modify its innerHTML using `document.getElementById()`.  This check prevents errors and ensures the script behaves correctly even when the target element is not found.