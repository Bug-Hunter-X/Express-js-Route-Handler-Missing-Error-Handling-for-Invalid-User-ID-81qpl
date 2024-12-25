# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input. Specifically, the code lacks checks for non-numeric user IDs, which can lead to crashes or unexpected results.

## Bug

The `bug.js` file contains an Express.js route handler that retrieves a user by ID.  It attempts to parse the ID as an integer but doesn't handle cases where the ID is not a number. This can lead to errors or unexpected results if a non-numeric ID is provided.

## Solution

The `bugSolution.js` file provides a corrected version of the route handler. It includes checks to ensure the user ID is a number before proceeding, preventing potential errors and providing a more robust solution.

## How to Run

1. Clone this repository.
2. Navigate to the directory.
3. Install dependencies: `npm install`
4. Run the application: `node bug.js` or `node bugSolution.js`