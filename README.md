# ts-eslint-error

A minimal reproduction of a ts-eslint-error.

Seeing the error:

```sh
npm install
npx ts-standard
```

Output:

```text
ts-standard: Standard for TypeScript! (https://github.com/standard/ts-standard)
  /Users/meyerdom/Projekte/Privat/TsStandardError/test.ts:0:0: Parsing error: ESLint was configured to run on `<tsconfigRootDir>/test.ts` using `parserOptions.project`: /users/meyerdom/projekte/privat/tsstandarderror/tsconfig.json
However, that TSConfig does not include this file. Either:
- Change ESLint's list of included files to not include this file
- Change that TSConfig to include this file
- Create a new TSConfig that includes this file and include it in your parserOptions.project
See the typescript-eslint docs for more info: https://typescript-eslint.io/linting/troubleshooting#i-get-errors-telling-me-eslint-was-configured-to-run--however-that-tsconfig-does-not--none-of-those-tsconfigs-include-this-file (null)
```
