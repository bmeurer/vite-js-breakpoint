# Repro for breakpoints in JS preserved by Vite HMR

Start via:

```
npm install
npm run dev
```

Set a breakpoint in `counter.js` (inside `setCounter()` function), and notice that it hits.
Now modify `counter.js` and wait for the HMR to happen, and notice that the breakpoint is
gone ([vitejs/vite#13503](https://github.com/vitejs/vite/issues/13503)).
