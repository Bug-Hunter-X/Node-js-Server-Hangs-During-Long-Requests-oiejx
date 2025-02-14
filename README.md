# Node.js Server Hang Issue

This repository demonstrates a common issue in Node.js applications where the server becomes unresponsive during long-running requests.  The provided code simulates a scenario where a request takes 5 seconds to process, blocking the event loop and preventing the server from handling other requests.  The solution shows a method to resolve this using asynchronous operations.

## Steps to Reproduce
1. Clone the repository.
2. Run `node server.js`.
3. Make a request to `http://localhost:3000`.  Notice that the server will hang and not respond to further requests while processing this request.

## Solution
The solution utilizes asynchronous operations and the `setTimeout` function to avoid blocking the event loop.