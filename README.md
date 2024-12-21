# React useEffect setInterval Memory Leak

This repository demonstrates a common error in React applications involving the `useEffect` hook and `setInterval`. The example shows how an improper implementation of `setInterval` within `useEffect` can lead to memory leaks.

## Problem
The `setInterval` function, when used without proper cleanup, continues to run even after the component unmounts. This consumes resources and can negatively impact performance. The provided `bug.js` file demonstrates this issue.

## Solution
The `bugSolution.js` file provides a corrected implementation.  It utilizes a cleanup function within the `useEffect` hook to clear the `setInterval` when the component is unmounted, preventing the memory leak.

## How to run
1. Clone this repository.
2. Navigate to the directory in your terminal.
3. Run `npm install`.
4. Run `npm start` (assuming a suitable React development environment).
