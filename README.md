# Unhandled Promise Rejection in Express.js Route

This repository demonstrates a common error in Express.js applications: unhandled promise rejections within asynchronous route handlers.  When an asynchronous operation within a route fails and the error isn't properly handled, it can lead to silent failures, making debugging difficult and potentially impacting the user experience.

The `bug.js` file contains code that reproduces this error.  The `bugSolution.js` file provides a corrected version with appropriate error handling.

## How to Reproduce

1. Clone this repository.
2. Navigate to the repository's directory.
3. Run `node bug.js`.
4. Observe that errors are logged to the console, but the client receives no error response.
5. Run `node bugSolution.js` to see the corrected version, which returns error responses to the client.