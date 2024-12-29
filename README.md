# Express.js Unhandled Error Bug

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling for invalid input or missing resources.

The `bug.js` file contains the erroneous code.  It attempts to fetch a user from an array using a user ID passed as a route parameter. However, it fails to gracefully handle cases where the ID is not a number or no user with that ID exists. 

The `bugSolution.js` file provides a corrected version with improved error handling. It checks if the ID is a number and returns a 404 Not Found error if the user is not found.