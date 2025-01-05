# Prompt for Creating Unit Tests for a Node.js File with Jest Configuration and Error Handling

Create unit tests for the following Node.js file. Ensure the following guidelines are met:

1. **Testing Framework:**  
   Use the [Jest](https://jestjs.io/) framework for unit tests. If Jest is not already installed, include instructions to install it with:
   ```bash
   npm install --save-dev jest
   ```

2. **Configure Jest:**  
   - Check if a `jest.config.js` file exists in the project. If it does not exist, create one with default configurations.  
   - Ensure the configuration supports `.mjs` files and aligns with ES6 modules. Update `jest.config.js` if necessary. For example:
     ```javascript
     export default {
         transform: {},
         testEnvironment: 'node',
         moduleFileExtensions: ['js', 'mjs'],
     };
     ```

3. **Test All Functions:**  
   Write comprehensive unit tests to cover all exported functions, methods, or classes in the given file. Include:
   - Positive test cases.
   - Negative test cases.
   - Edge cases and invalid inputs.

4. **Mock Dependencies:**  
   If the file relies on external modules, APIs, or libraries, use mocks or stubs to isolate the functionality being tested.

5. **File Naming and Saving:**  
   - Name the test file with a `.test.mjs` extension, following the convention of the original file. For example, if the file is `example.mjs`, the test file should be named `example.test.mjs`.  
   - Save the generated test file in a `tests` folder located at the root of the project. For example:
     ```
     tests/
     └── example.test.mjs
     ```

6. **Include Setup and Teardown:**  
   Use Jest's `beforeEach` and `afterEach` hooks for setup and teardown logic if needed.

7. **Organized Test File:**  
   Structure the test file using `describe` and `test` blocks to group related tests together. Ensure the tests are readable and follow best practices.

8. **Run and Verify Tests:**  
   - After writing the tests, run them using:
     ```bash
     npm test
     ```
   - Check for any errors or failed tests. If errors occur, provide corrections for the Node.js file or the test file to resolve them.

9. **Error Handling and Correction:**  
   - If errors or failed tests are detected during `npm test`, analyze the errors and correct them automatically.  
   - Prompt:  
     *"Errors were found during testing. Would you like me to correct the issues in the test file or the source file?"*  
   - Make the necessary corrections and re-run the tests to ensure all errors are resolved.

10. **Ensure Full Coverage:**  
    Ensure all exported functions and logical branches in the Node.js file are tested. Generate a coverage report if needed by adding this to the `jest.config.js`:
    ```javascript
    collectCoverage: true,
    coverageDirectory: 'coverage',
    ```

## Example Test Workflow:
1. **Given Node.js File:**
   ```javascript
   export function add(a, b) {
       return a + b;
   }
   ```

2. **Generated Test File (`tests/add.test.mjs`):**
   ```javascript
   import { add } from '../add.mjs';

   describe('add function', () => {
       test('should return the sum of two numbers', () => {
           expect(add(1, 2)).toBe(3);
       });

       test('should throw an error for invalid inputs', () => {
           expect(() => add(1, null)).toThrow();
       });
   });
   ```

3. **Run Tests:**  
   Execute:
   ```bash
   npm test
   ```

4. **Handle Errors:**  
   If any errors or test failures occur, Copilot should analyze the errors and provide fixes for both the test and source files.

## Node.js File to Create Tests For:
```javascript
<paste your Node.js file here>
```