# Node.js Server Unresponsiveness

This repository demonstrates a common issue in Node.js where a server becomes unresponsive due to a long-running synchronous operation within the request handler.  The `bug.js` file contains the problematic code, which uses a `while` loop to simulate a time-consuming task. This blocks the event loop, preventing the server from responding to subsequent requests.

The solution, `bugSolution.js`, demonstrates how to resolve this by using asynchronous operations or offloading the work to a worker thread.