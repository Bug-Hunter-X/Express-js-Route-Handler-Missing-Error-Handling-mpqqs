# Express.js Route Handler Missing Error Handling

This repository demonstrates a common error in Express.js route handlers:  the lack of proper error handling when dealing with user input.  The example shows a route that fetches a user by ID.  The original code fails to handle cases where the ID is invalid (not a number) or the user doesn't exist.  The solution shows how to add error handling to gracefully handle these situations.

## Bug

The `bug.js` file contains the flawed code.  The main issue is the absence of error handling when parsing the `userId` and when the user is not found. This can lead to unexpected crashes or 500 errors.