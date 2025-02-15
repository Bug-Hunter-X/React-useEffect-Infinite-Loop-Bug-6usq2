# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug occurs when the dependency array for `useEffect` is incorrect, leading to an infinite render loop.

The `bug.js` file contains the buggy code. The `bugSolution.js` file provides the corrected version.

## Bug Description

The `useEffect` hook, when not given the proper dependency array, can cause the component to re-render indefinitely, resulting in performance issues and potential crashes.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` (or `yarn install`).
3. Run `npm start` (or `yarn start`).
4. Observe the infinite console logs and the browser becoming unresponsive.

## Solution

The solution involves carefully specifying the dependencies in the `useEffect` hook's second argument. Missing even one value can lead to the problem demonstrated here.  The corrected code is in the `bugSolution.js` file.