# Unhandled 'error' event in Node.js Server
This repository demonstrates a common yet often overlooked error in Node.js server development: the unhandled 'error' event.  When a server attempts to bind to an occupied port, it typically crashes silently without informative error messages.  This example shows how to gracefully handle this situation.

## Bug
The `bug.js` file contains a simple HTTP server that listens on port 3000. If this port is already in use, the server will crash without proper error handling. 

## Solution
The `bugSolution.js` file demonstrates the correct way to handle the 'error' event, providing a more robust and user-friendly experience. 