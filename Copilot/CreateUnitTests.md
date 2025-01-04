# Prompt for Creating Unit Tests for a Node.js File

Create unit tests for the following Node.js file. Ensure the following guidelines are met:

1. **Testing Framework:**  
   Use the [Jest](https://jestjs.io/) framework for the unit tests.

2. **Test All Functions:**  
   Write comprehensive unit tests to cover all exported functions, methods, or classes in the given file. Include both positive and negative test cases for edge cases and invalid inputs.

3. **Mock Dependencies:**  
   If the file relies on external modules, APIs, or libraries, use mocks or stubs to isolate the functionality being tested.

4. **Maintain Naming Conventions:**  
   Ensure the test descriptions and structure follow best practices and clearly describe the functionality being tested.

5. **Include Setup and Teardown:**  
   If necessary, include setup and teardown logic using Jest's `beforeEach` and `afterEach` hooks.

6. **Organized Test File:**  
   Place the tests in a structured format using `describe` and `test` blocks to group related tests together.

7. **File Naming and Saving:**  
   - Name the test file with `.test.js` or `.spec.js` extension, following the convention of the original file. For example, if the file is `example.mjs`, the test file should be named `example.test.js`.  
   - Save the generated test file in a `tests` folder located at the root of the project. For example:
     ```
     tests/
     └── example.test.js
     ```

8. **Code Example:**  
   For example, if the Node.js file contains:
   ```javascript
   export function add(a, b) {
       return a + b;
   }
   ```
   The test should look like:
   ```javascript
   import { add } from '../filename';

   describe('add function', () => {
       test('should return the sum of two numbers', () => {
           expect(add(1, 2)).toBe(3);
       });

       test('should throw an error for invalid inputs', () => {
           expect(() => add(1, null)).toThrow();
       });
   });
   ```

9. **Ensure Full Coverage:**  
   Provide tests for all edge cases and ensure all branches of the logic in the Node.js file are tested.

10. **Save All Tests in a `tests` Folder:**  
    Ensure all generated test files are saved in a `tests` folder at the root of the project to keep the project organized.

Here is the Node.js file to create tests for:
```javascript
<paste your Node.js file here>
```