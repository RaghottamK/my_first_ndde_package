# my_first_ndde_package
### RK_Add_Operation Package

### More around documentation

https://docs.npmjs.com/creating-node-js-modules


1. run npm init
2. Provide responses for the required fields (name and version), as well as the main field:
name: The name of your module.
version: The initial module version. We recommend following [semantic versioning](https://docs.npmjs.com/about-semantic-versioning) guidelines and starting with 1.0.0
3. Create the file, add a function as a property of the exports object.

```
exports.printMsg = function() {
  console.log("This is a message from the demo package");
}
```

4. Publish your packages to npm <br/>
    For private packages - use `npm publish` <br />
    For public packages, use `npm publish --access public`

5. Create a new test directory outside your project directory to test your package
`mkdir test-your-package`

6. Switch to new directory and install your module:
    `npm install <your-module-name>`
7. Call your module method
    ```
    const addTwoNumbers = require('rk_add_operation');
    console.log(addTwoNumbers(5, 10));
    ```
8. From cmd line run below to print the result <br />
    `node test.js`