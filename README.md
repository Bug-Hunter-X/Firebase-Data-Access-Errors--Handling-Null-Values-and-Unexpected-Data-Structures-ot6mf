# Firebase Data Access Errors: Handling Null Values and Unexpected Data Structures

This repository demonstrates a common error in Firebase applications: attempting to access data that is null or undefined, or which is not structured as expected. This can lead to runtime errors and unexpected behavior.

## Problem
The `bug.js` file contains code that attempts to access a property from a Firebase snapshot. If the data structure is not as expected, or if the property does not exist, a runtime error occurs.

## Solution
The `bugSolution.js` file provides a robust solution using optional chaining and nullish coalescing to safely handle potential null or undefined values.  Error handling is implemented to gracefully handle situations where the expected data isn't present.

## How to run
1.  Clone this repository.
2.  Install the Firebase SDK (`npm install firebase`).
3.  Set up your Firebase project and configure the `firebaseConfig` object in the code.
4. Run `node bug.js` and `node bugSolution.js` to compare the error-prone and robust versions.