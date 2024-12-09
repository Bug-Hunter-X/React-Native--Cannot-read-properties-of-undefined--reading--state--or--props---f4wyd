# React Native: Cannot read properties of undefined (reading 'state' or 'props')

This repository demonstrates a common React Native bug and its solution. The bug occurs when you attempt to access component state or props before the component has fully mounted.  The solution illustrates how to ensure these values are available before accessing them.

## Bug

The `Bug.js` file showcases the problematic code.  It attempts to read a prop or state variable within the `constructor`, which is too early in the component lifecycle.

## Solution

The `BugSolution.js` file corrects the issue by moving the access of state or props to `componentDidMount` or by using conditional rendering to check if state or props exist.