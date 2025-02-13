# Infinite Rendering Bug in React

This repository demonstrates a common bug in React applications: infinite rendering caused by a missing dependency array in the `useEffect` hook.  The `MyComponent` initially renders correctly, but subsequently enters an infinite render loop, overwhelming the browser.

## Bug Description
The `useEffect` hook in `bug.js` lacks a dependency array. This causes the effect to run after every render, triggering a state update that leads to another render, creating an infinite loop.