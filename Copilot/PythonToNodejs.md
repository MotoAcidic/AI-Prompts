## Comprehensive Prompt for Copilot:

* Convert the following Python code into JavaScript .mjs format. Ensure the following guidelines are met:

* Preserve Comments: Retain all comments from the original Python file and place them in the appropriate sections of the JavaScript code. Adjust comments if necessary to align with JavaScript syntax or conventions.

* Maintain Naming Conventions: Use the same naming conventions for functions, variables, and classes as in the Python code. This is crucial for compatibility with other files that rely on these names.

* Replace Python Libraries: Identify and use equivalent JavaScript libraries or npm packages to replicate the functionality of Python-specific libraries and functions.

* Convert Example Usage: If the Python file contains example usage or demonstration code (anywhere in the file), fully translate it into JavaScript code. However, ensure the translated example usage code is commented out in the JavaScript file so it does not interfere with runtime execution or compilation. For example:

``` javascript
// Example usage:
// const result = process_data(inputData);
// console.log(result);
```

* Use ES6 Syntax: Utilize modern ES6+ features such as import/export for module management and arrow functions where appropriate.

* Functional Code: Ensure the converted JavaScript code is logically consistent with the original Python code and functional with the equivalent JavaScript libraries.

* Locate Example Usage: Search through the entire file for any example usage sections or demonstration code, and translate them into fully implemented JavaScript examples, ensuring they are commented out in the .mjs file.