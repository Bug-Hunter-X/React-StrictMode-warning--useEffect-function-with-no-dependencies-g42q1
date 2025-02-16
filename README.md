# React StrictMode Warning: useEffect with no dependencies

This example demonstrates a common warning encountered when using React's StrictMode.  The `useEffect` hook without a dependency array can lead to unexpected behavior and performance issues.

## Problem
The `useEffect` hook in `bug.js` is called after every render. In StrictMode this causes double calls or warnings to console log. To avoid this, add an empty dependency array to the useEffect hook.

## Solution
The `bugSolution.js` file shows the corrected code, adding an empty array `[]` as the second argument to `useEffect` to ensure it only runs once after the initial render.