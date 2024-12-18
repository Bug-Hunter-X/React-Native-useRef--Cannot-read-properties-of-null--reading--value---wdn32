# React Native useRef Null Error

This repository demonstrates a common error in React Native when using the `useRef` hook: attempting to access the current value of a ref before it's been assigned.  This often leads to a `Cannot read properties of null (reading 'value')` error.

The `bug.js` file shows the problematic code, and `bugSolution.js` provides a corrected version.  The issue arises because accessing `inputRef.current` before the component mounts results in null.

The solution is to ensure the ref is accessed only after the component has rendered and the ref has been assigned a value.