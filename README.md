Reproduction for https://github.com/vitejs/vite/issues/21088.  
Original issue: https://github.com/vikejs/vike/issues/2823.  

Error:

```
9:20:45 PM [vite] Failed to transpile /node_modules/.vite/deps/chunk-ALJFZQEA.js because:
Failed to resolve import "@brillout/picocolors" from "node_modules/.vite/deps/chunk-ALJFZQEA.js?v=83d14f49". Does the file exist?
48 |  
49 |  // node_modules/.pnpm/telefunc@0.2.15_@babel+core@7.28.5_@babel+parser@7.28.5_@babel+types@7.28.5_react-strea_b67ab6a...
50 |  import pc from "@brillout/picocolors";
   |                  ^
51 |  var errorPrefix = `[telefunc@${projectInfo.projectVersion}]`;
52 |  var internalErrorPrefix = red(`${errorPrefix}[Bug]`);
```

Reprodution steps:

```
pnpm i
pnpm run dev
```

Then go to http://localhost:3000/todo
