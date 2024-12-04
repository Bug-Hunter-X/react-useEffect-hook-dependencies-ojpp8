# React useEffect Hook Dependency Array Issue

This example demonstrates a common mistake when using the `useEffect` hook in React. The effect runs more often than intended because the dependency array is incorrect.

## Bug
The `useEffect` hook in `bug.js` is intended to log the current value of `count` whenever it changes. However, because of the missing dependency, it runs after every render, causing unexpected behavior and potentially performance issues.

## Solution
The corrected code in `bugSolution.js` addresses this problem by including `count` in the dependency array. Now, the effect only runs when the `count` variable actually changes, leading to efficient behavior.
