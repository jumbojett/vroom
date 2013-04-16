Vroom for Elgg
==================
A simple way to speed up elgg. Vroom operates by flushing the output buffer before elgg shutdown begins. The browser is able to render results quickly to the user while additional shutdown functions continue on the server uninterrupted. Vroom can be used in conjunction with process intensive elgg internals such as notifications to create a more user-friendly atmosphere. 

## Features
 - Lighting fast elgg execution

## Server requirements
 - Elgg 1.8.3 or greater

## Developers

### Converting code


### Shutdown state
Vroom sets a global `shutdown_flag` to let functions know if elgg is in shutdown mode. This can be checked easily. For example:  `isset($GLOBALS['shutdown_flag'])` 
