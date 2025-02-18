# Inefficient and Unsafe innerHTML Concatenation in HTML

This repository demonstrates an uncommon but important HTML bug related to the inefficient and potentially insecure use of `innerHTML`.  Repeatedly concatenating strings with `innerHTML` can impact performance, particularly with large amounts of data.  Furthermore, it introduces security risks if unsanitized user input is added.

## Bug Description
The `bug.html` file showcases this issue. It appends new paragraphs to a div element by repeatedly concatenating to the `innerHTML` property.  This approach is less efficient than other methods.

## Solution
The `bugSolution.html` file provides a more efficient and safer alternative, using `insertAdjacentHTML` for appending content.

## How to run
Simply open the HTML files in a web browser to observe the behavior.