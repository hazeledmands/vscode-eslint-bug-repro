Reproducing https://github.com/microsoft/vscode-eslint/issues/1047

Run:
```
npm install
npm run lint
```

And you'll get the following output:
```
eslint-config-test/index.ts
  2:28  error  Missing semicolon  semi

✖ 1 problem (1 error, 0 warnings)
  1 error and 0 warnings potentially fixable with the `--fix` option.
```

However, if you open `index.ts` with Visual Studio Code (and have the [`vscode-eslint` plugin](https://github.com/microsoft/vscode-eslint) enabled) you will not see this error highlighted.