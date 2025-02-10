# React useEffect Cleanup Bug

This repository demonstrates a common React bug involving memory leaks due to a missing cleanup function within the `useEffect` hook.  The `bug.js` file contains the erroneous code, while `bugSolution.js` provides the corrected version.

**Bug Description:**
The component adds an event listener but forgets to remove it when the component unmounts. This causes a memory leak.

**Solution:**
The `useEffect` hook's return value should be a cleanup function that removes the event listener.