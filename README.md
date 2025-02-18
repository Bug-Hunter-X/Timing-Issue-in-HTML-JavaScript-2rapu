# Uncommon HTML Bug: DOM Timing Issue
This repository demonstrates a subtle timing bug in HTML/JavaScript where a script attempts to modify a DOM element before it's fully loaded. This can lead to unexpected behavior such as the script not having the desired effect.

## Bug Description
The HTML file contains a `div` element with some text. A JavaScript script attempts to hide this `div` by changing its `display` style to "none". However, if the script executes before the DOM element is fully loaded, the change won't take effect.

## Solution
The solution involves using the `DOMContentLoaded` event, which ensures that the script runs after the entire HTML document has been parsed and is ready.