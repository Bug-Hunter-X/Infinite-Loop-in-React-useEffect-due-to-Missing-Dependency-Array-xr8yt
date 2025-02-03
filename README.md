# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook.  The `useEffect` hook, without a dependency array, runs after every render, creating an infinite loop and causing performance issues. This example highlights the problem and shows how to fix it by correctly specifying dependencies.

## Bug
The `bug.js` file contains a component that uses `useEffect` without specifying a dependency array. This leads to the effect running on every render, causing an infinite loop of re-renders and console log outputs.

## Solution
The `bugSolution.js` file demonstrates the correct use of the dependency array.  By including `count` in the dependency array, the effect only runs when the `count` value changes, resolving the infinite loop.