# Unnecessary useEffect Re-renders in React

This repository demonstrates a common React performance issue: unnecessary re-renders caused by useEffect hooks.

## Problem

The `MyComponent` in `bug.js` uses `useEffect` without specifying dependencies. This means the effect runs after every render.  The console log shows this continuous execution.

## Solution

The `bugSolution.js` shows the fix by adding the `count` variable as dependency.  The effect will only run when the `count` variable changes. 

## How to Run

1. Clone the repository.
2. Navigate to the repository directory.
3. Run `npm install`.
4. Run `npm start`.

## Note

This example illustrates how using the dependency array in `useEffect` significantly improves the performance of React components by preventing unnecessary re-renders.