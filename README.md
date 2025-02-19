# Unhandled Exception in Node.js HTTP Server

This repository demonstrates a common error in Node.js applications: insufficient error handling in HTTP servers.  The `bug.js` file shows a server that lacks proper error handling, causing it to crash silently upon encountering unexpected issues.

The `bugSolution.js` file provides a corrected version with robust error handling, preventing crashes and providing informative error messages.

## How to Reproduce the Bug

1. Clone this repository.
2. Run `node bug.js`.
3. Observe that the server starts successfully.
4. Attempt to trigger an error (e.g., by sending a malformed request). The server will crash without any indication of what happened. 

## How to Run the Solution

1. Run `node bugSolution.js`
2. Attempt to trigger an error. This time, the server will log an error to the console and gracefully continue operation, preventing service interruption.