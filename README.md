# Uncommon HTML Bug: innerHTML unexpected behavior with number concatenation

This repository demonstrates an uncommon bug related to using innerHTML in HTML when concatenating strings with numbers.

The `bug.html` file contains code that attempts to modify the content of a div element.  The `innerHTML` property is used to set the new content, but a number is concatenated to the end of the string. This concatenation leads to unexpected behavior.  The solution, provided in `bugSolution.html`, addresses this by properly handling the string and number concatenation within `innerHTML`.

## Bug Description:
When using innerHTML to set the content of an HTML element, and you are appending a number to the string that will be inserted as HTML, the number is treated as text, not as a numerical value.  This may cause unexpected behavior depending on the surrounding HTML.   This is because the browser interprets the `innerHTML` property's value as HTML.  Therefore, you have to create the appropriate HTML using string templates or by carefully forming the HTML string.