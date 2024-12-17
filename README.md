# React useEffect Hook: Missing Dependency in Dependency Array

This repository demonstrates a common error in React's `useEffect` hook: omitting necessary dependencies from the dependency array.  This can lead to unexpected behavior and performance issues.

## The Bug

The `bug.js` file contains a `useEffect` hook that's missing the `count` variable in its dependency array. This causes the effect to run on every render, regardless of whether `count` has changed. This can lead to unnecessary re-renders and potential performance problems, particularly in complex applications.

## The Solution

The `bugSolution.js` file demonstrates the correct usage of the `useEffect` hook. By adding `count` to the dependency array, the effect now only runs when the value of `count` changes, preventing unnecessary re-renders.

## How to Run

1. Clone this repository.
2. Navigate to the project directory using a terminal.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.