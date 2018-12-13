This shows typewiz-node inserting type info at incorrect offsets into files 
when using the given run.js script.  The script is based on the one from 
https://github.com/urish/typewiz-node-no-apply.

To repro:

```
yarn
yarn ts-node run.js
yarn typewiz applyTypes collected-types.json
cat a.ts
```
