#### Testing Project

This project demonstrates the steps to build and use an npm package. The package, named `testing`, provides a simple `helloWorld` function that returns the string "Hello, World!".

##### Project Structure

- **index.js**: Entry point of the project.
- **package.json**: Contains metadata about the project and its dependencies.
- **test-package/**: Directory containing test files.
- **test-package/test.js**: Test file that requires and uses the `testing` package.

##### Installation

To install the dependencies, run:

```sh
npm install
```

##### Usage

To use the helloWorld function from the testing package, you can require it in your JavaScript files:

```js
const testing = require("testing");
console.log(testing.helloWorld());
```

##### Testing

To run the tests, execute:

```sh
cd test-package
node test.js
```

##### Development

To develop and test the package locally, follow these steps:

1. Navigate to the package directory:

```sh
cd path/to/your/package
```

2. Install the dependencies:

```sh
npm install
```

3. Link the package globally:

```sh
npm link
```

4. Navigate back to your project directory and link the `testing`package:

```sh
cd path/to/your/project
npm link testing
```

5. Run the test script:

```sh
node test-package/test.js
```

##### License

This project is licensed under the ISC License - see the LICENSE file for details.

##### Author

Prince Kumar Prasad