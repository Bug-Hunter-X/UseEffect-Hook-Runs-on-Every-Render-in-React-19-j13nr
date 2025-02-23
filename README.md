# useEffect Hook Runs on Every Render in React 19

This repository demonstrates a common issue with the `useEffect` hook in React 19 where the effect runs on every render even when an empty dependency array is provided. This is usually because of incorrect usage of the hook, such as indirectly accessing state or props that change on every render within the effect's logic.  The solution involves carefully examining state and prop usage inside the useEffect function. 

## Bug Description
The provided `useEffect` hook is intended to log a message only once. However, in this example, it logs on every render.