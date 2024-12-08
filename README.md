# Express.js - Missing JSON.stringify in response

This repository demonstrates a common error in Express.js applications where an object is sent as a response without being stringified first using `JSON.stringify()`. This results in a non-JSON response and can cause errors on the client-side.

## Bug
The `bug.js` file contains the erroneous code.  The response to a GET request at `/users/:id` sends a JavaScript object directly to the client without stringification.

## Solution
The `bugSolution.js` file shows the correct way to send JSON responses in Express.js, which is to stringify the object using `JSON.stringify()` before sending it.
