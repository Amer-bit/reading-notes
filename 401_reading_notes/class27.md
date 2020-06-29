# Jest and Testing
Jest is a Node-based runner. This means that the tests always run in a Node environment and not in a real browser. This lets us enable fast iteration speed and prevent flakiness.

While Jest provides browser globals such as window thanks to jsdom, they are only approximations of the real browser behavior. Jest is intended to be used for unit tests of your logic and your components rather than the DOM quirks.

## Filename Conventions

Jest will look for test files with any of the following popular naming conventions:

* Files with .js suffix in __tests__ folders.
* Files with .test.js suffix.
* Files with .spec.js suffix.

It's recommended to put the test files (or __tests__ folders) next to the code they are testing so that relative imports appear shorter. Collocation also helps find tests more quickly in larger projects.

## Version Control Integration
By default, when you run npm test, Jest will only run the tests related to files changed since the last commit. This is an optimization designed to make your tests run fast regardless of how many tests you have. However it assumes that you don’t often commit the code that doesn’t pass the tests.

Jest will always explicitly mention that it only ran tests related to the files changed since the last commit. You can also press a in the watch mode to force Jest to run all tests.

## Writing Tests
To create tests, add it() (or test()) blocks with the name of the test and its code. **You may optionally wrap them in describe() blocks for logical grouping but this is neither required nor recommended.**

## Testing Components
There is a broad spectrum of component testing techniques. They range from a **“smoke test”** verifying that a component renders without throwing, to **shallow rendering** and testing some of the output, to **full rendering and testing component lifecycle and state changes**.

Different projects choose different testing tradeoffs **based on how often components change, and how much logic they contain.** If you haven’t decided on a testing strategy yet, we recommend that you start with creating basic smoke tests for your components.

## Shallow rendering
Shallow rendering is useful to constrain yourself to testing a component as a unit, and to ensure that your tests aren't indirectly asserting on behavior of child components. **It's recommended using shallow() rendering API from Enzyme.**

