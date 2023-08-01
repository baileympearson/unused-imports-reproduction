# unused-imports-reproduction

This repository reproduces a bug in api-extractor where api-extractor emits unused imports after stripping internal types.

To reproduce:

1. clone this repo
2. `npm install`
3. `npm run build`
4. Open the generated file and notice that the field marked internal has been stripped from the types, but the import for `MongoCrypt` remains and is unused.
