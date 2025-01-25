# React Router Dom v6 Catch-all Route Bug

This repository demonstrates a bug in React Router Dom v6 where the catch-all route (`/*`) is triggered even when a valid route exists.  The issue arises from the order of routes defined within the `Routes` component.  The catch-all route should only be triggered when no other routes match.

## Bug

The provided `bug.js` file shows the incorrect implementation where the catch-all route overrides other defined routes.

## Solution

The `bugSolution.js` file demonstrates the correct implementation, placing the catch-all route as the last route defined within the `Routes` component.