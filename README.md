# Express.js Unhandled POST Request Error

This repository demonstrates a common error in Express.js applications: the lack of proper error handling for POST requests.  The provided code lacks checks for missing or malformed data in the request body, resulting in potential server crashes or unexpected responses.

The `bug.js` file shows the faulty code, while `bugSolution.js` presents the corrected version with improved error handling.

## How to Reproduce

1. Clone the repository.
2. Navigate to the repository's directory.
3. Run `npm install` to install dependencies.
4. Run `node bug.js`. 
5. Send a POST request to `http://localhost:3000/user` with a missing or invalid JSON body.  Observe the behavior.
6. Repeat steps 4 and 5, but use `node bugSolution.js` and observe the improvement.

## Solution

The solution involves adding comprehensive checks to validate the incoming request data before processing it.  This prevents errors caused by unexpected input.  Always validate user inputs!