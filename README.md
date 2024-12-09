# React Native: undefined is not an object (evaluating 'this.state.data')
This repository demonstrates a common React Native error: `undefined is not an object (evaluating 'this.state.data')`.  This occurs when trying to access a state variable before it's been assigned a value, frequently during asynchronous operations.

The `bug.js` file shows the problematic code.  `bugSolution.js` provides a solution using conditional rendering to avoid accessing the state before it's ready.

## How to reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run the app in your React Native environment.
4. Observe the error in the console (or lack of error with the solution implemented).

## Solution
The key is to ensure data is fetched and assigned to the state *before* attempting to render it.  This often involves using a loading state and conditional rendering.