# Prompt for Converting Python Code into JavaScript `.mjs` Format

Convert the following Python code into JavaScript `.mjs` format. Ensure the following guidelines are met:

1. **Preserve Comments:**  
   Retain all comments from the original Python file and place them in the appropriate sections of the JavaScript code. Adjust comments if necessary to align with JavaScript syntax or conventions.

2. **Preserve Commented-Out Code:**  
   Any functions, blocks of code, or logic that are commented out in the original Python file must remain in the JavaScript file, translated into `.mjs` format and commented out to maintain the full integrity of the original file.  

   For example:  
   ```python
   # def commented_out_function(x):
   #     return x * 2
   ```  
   Should be converted to:  
   ```javascript
   // function commented_out_function(x) {
   //     return x * 2;
   // }
   ```

3. **Maintain Naming Conventions:**  
   Use the same naming conventions for functions, variables, and classes as in the Python code. This is crucial for compatibility with other files that rely on these names.

4. **Avoid Reserved Words as Parameter Names:**  
   Ensure that no parameter in any function has the same name as a reserved word in JavaScript. Reserved words like `function` and `package` cannot be used as parameter names. Rename such parameters if necessary to avoid conflicts, while maintaining code clarity. For example:
   ```python
   # def some_function(package):
   #     return package + 1
   ```
   Should be converted to:
   ```javascript
   // function some_function(pkg) {
   //     return pkg + 1;
   // }
   ```

5. **Replace Python Libraries:**  
   Identify and use equivalent JavaScript libraries or npm packages to replicate the functionality of Python-specific libraries and functions. Include the necessary `import` statements for these libraries.

6. **Convert Example Usage:**  
   If the Python file contains example usage or demonstration code (anywhere in the file), fully translate it into JavaScript code. However, ensure the translated example usage code is commented out in the JavaScript file so it does not interfere with runtime execution or compilation.  

   For example:  
   ```python
   # Example usage:
   # result = process_data(input_data)
   # print(result)
   ```  
   Should be converted to:  
   ```javascript
   // Example usage:
   // const result = process_data(inputData);
   // console.log(result);
   ```

7. **Use ES6 Syntax:**  
   Utilize modern ES6+ features such as `import`/`export` for module management and arrow functions where appropriate.

8. **Functional Code:**  
   Ensure the converted JavaScript code is logically consistent with the original Python code and functional with the equivalent JavaScript libraries. Make sure the final code is fully compatible with JavaScript runtime and adheres to modern JavaScript best practices.

9. **Locate Example Usage:**  
   Search through the entire file for any example usage sections or demonstration code. Translate them into fully implemented JavaScript examples, ensuring they are commented out in the `.mjs` file to avoid interfering with runtime execution.

10. **Incremental Conversion for Large Files:**  
    - Break down the Python code into logical sections (e.g., functions, classes, or modules) and convert each section step by step.  
    - After completing each section, indicate whether:  
      - The conversion for that section is complete.  
      - There are more sections to convert. Prompt:  
        *"There is more to convert. Do you want me to continue?"*  
      - If the full file has been converted, confirm with:  
        *"The entire file has been converted. There is nothing else to convert."*  
    - Wait for confirmation before proceeding to the next section.

## Python Code to Convert:
```python
<paste your Python code here>
```