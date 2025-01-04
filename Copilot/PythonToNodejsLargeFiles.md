# Prompt for Converting Large Files Using Copilot

Convert the following Python code into JavaScript `.mjs` format in manageable increments. Follow these guidelines:

1. **Incremental Conversion:**  
   Break down the Python code into logical sections (e.g., functions, classes, or modules) and convert each section step by step. Do not attempt to convert the entire file at once.

2. **Preserve Comments:**  
   Retain all comments from the original Python file in each increment and ensure they are placed appropriately in the corresponding JavaScript code.

3. **Maintain Naming Conventions:**  
   Use the same naming conventions for functions, variables, and classes as in the Python code.

4. **Replace Python Libraries:**  
   Identify equivalent JavaScript libraries for Python-specific libraries and functions, and include the necessary `import` statements for each section.

5. **Example Usage Conversion:**  
   If a section includes example usage code, translate it into JavaScript, but ensure it is commented out in the `.mjs` file to avoid interfering with runtime execution. For example:
   ```javascript
   // Example usage:
   // const result = process_data(inputData);
   // console.log(result);
   ```

6. **Pause Between Sections:**  
   After completing each section, pause and indicate that the section is complete. Then wait for the next instruction to continue with the next part of the file.

7. **Complete Full File:**  
   Ensure the entire file is fully converted by proceeding section by section until the task is complete. Prompt me if clarification is needed for a specific section.

## Usage Instructions for Large Files
1. **Start Conversion:**  
   Provide the Python code with the above prompt. Copilot will begin converting the first section.

   - Example response from Copilot:  
     *"Converted the first section of the file. Ready to proceed with the next section."*

2. **Continue Conversion:**  
   Use the following prompt to continue:  
   ```markdown
   Continue converting the next section of the Python code, following the same guidelines as before.
   ```

3. **Repeat Until Complete:**  
   Repeat the process until the entire file is converted.

## Python Code to Convert:
```python
<paste your Python code here>
```
