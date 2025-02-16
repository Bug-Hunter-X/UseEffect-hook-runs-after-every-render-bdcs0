# React useEffect Hook Runs After Every Render

This repository demonstrates a common issue with the React `useEffect` hook where it runs after every render instead of only when specified dependencies change.  This can lead to performance issues and unexpected behavior.

## Bug Description

The provided code demonstrates an `useEffect` hook that logs the current count to the console.  Even though the dependency array `[count]` is specified, the effect still runs after every render. 

## Solution

The issue is often related to closures or unintended re-renders that modify state implicitly, causing the effect to trigger.  The solution ensures proper state management and dependency tracking.  In the provided `bugSolution.js`, we correctly manage the dependency array. 
