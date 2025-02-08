# Stale Closure in useEffect Hook

This repository demonstrates a common React bug related to stale closures in the `useEffect` hook. The component attempts to log the current count every second. However, due to the closure capturing the initial value of `count`, it always logs 0, even though the state updates.