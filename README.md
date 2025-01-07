# React 19 useEffect Infinite Loop Bug

This repository demonstrates a common error in React 19 related to the `useEffect` hook.  Improperly defining dependencies in `useEffect` can lead to unexpected behavior, often resulting in an infinite loop.

The `bug.js` file showcases the problematic code.  The solution, implemented in `bugSolution.js`, correctly addresses the issue.

## Bug

The original code omits a crucial dependency in the `useEffect` hook. This omission causes the effect to run on every render, leading to an infinite loop because the state variable is updated inside the component.