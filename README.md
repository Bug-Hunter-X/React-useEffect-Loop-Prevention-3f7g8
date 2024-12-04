# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by a missing or incorrect dependency array.

## The Bug

The `bug.js` file contains a component that uses `useEffect` to log the count. However, the dependency array is missing or incomplete, causing the effect to run after every render, leading to an infinite loop.

## The Solution

The `bugSolution.js` file shows the corrected component.  The dependency array `[count]` ensures that the effect only runs when the `count` variable changes, preventing the infinite loop.