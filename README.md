# React useEffect Infinite Loop Bug
This repository demonstrates a common React bug involving the `useEffect` hook and its dependency array.  The component attempts to reset the count state to 0 on every render, leading to an infinite loop.  The solution provides the correct implementation.

## Bug
The `bug.js` file contains the erroneous code. The `useEffect` hook's dependency array is empty (`[]`), causing the effect to run after every render, resetting the `count` state to 0. This creates an infinite loop of renders and state updates.

## Solution
The `bugSolution.js` file shows the corrected code.  The dependency array is adjusted to only run the effect once on mount.  This fixes the infinite loop.