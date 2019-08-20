# ts-node-svg-filter-js

For reasons I don't understand, `ts-node` will fail to resolve the `@svgdotjs/svg.filter.js` npm dependency.

To see this for yourself, do the following:

```bash
git clone https://github.com/Lange/ts-node-svg-filter-js.git
cd ts-node-svg-filter-js
npm i
npm start
```

It should fail with an error like this: 

```
> Executing task: npm run start <


> ts-node-svg-filter@1.0.0 start c:\Users\vanca\Desktop\ts-node-svg-filter-js
> ts-node src/example.ts

Error: Cannot find module '@svgdotjs/svg.filter.js'
    at Function.Module._resolveFilename (internal/modules/cjs/loader.js:636:15)
    at Function.Module._load (internal/modules/cjs/loader.js:562:25)
    at Module.require (internal/modules/cjs/loader.js:692:17)
    at require (internal/modules/cjs/helpers.js:25:18)
    at Object.<anonymous> (c:\Users\vanca\Desktop\ts-node-svg-filter-js\src\example.ts:2:1)
    at Module._compile (internal/modules/cjs/loader.js:778:30)
    at Module.m._compile (c:\Users\vanca\Desktop\ts-node-svg-filter-js\node_modules\ts-node\src\index.ts:473:23)
    at Module._extensions..js (internal/modules/cjs/loader.js:789:10)
    at Object.require.extensions.(anonymous function) [as .ts] (c:\Users\vanca\Desktop\ts-node-svg-filter-js\node_modules\ts-node\src\index.ts:476:12)
    at Module.load (internal/modules/cjs/loader.js:653:32)
npm ERR! code ELIFECYCLE
npm ERR! errno 1
npm ERR! ts-node-svg-filter@1.0.0 start: `ts-node src/example.ts`
npm ERR! Exit status 1
npm ERR!
npm ERR! Failed at the ts-node-svg-filter@1.0.0 start script.
npm ERR! This is probably not a problem with npm. There is likely additional logging output above.

npm ERR! A complete log of this run can be found in:
npm ERR!     C:\Users\vanca\AppData\Roaming\npm-cache\_logs\2019-08-20T21_01_31_973Z-debug.log
The terminal process terminated with exit code: 1
```
