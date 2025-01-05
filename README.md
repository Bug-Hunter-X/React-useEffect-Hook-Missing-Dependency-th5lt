# React useEffect Hook Missing Dependency
This example demonstrates a common error in React's `useEffect` hook: a missing dependency in the dependency array. This can lead to unexpected behavior and subtle bugs. 

## Problem
The `useEffect` hook is designed to perform side effects after a component renders.  The dependency array determines when the effect runs.  If the dependency array is incorrect or missing, the effect may run unexpectedly or not run at all. 

In this case, the interval is set only once, during the initial render.  The counter will not update correctly. 

## Solution
The solution involves adding the `count` variable to the dependency array. This ensures the effect runs whenever the `count` value changes.
