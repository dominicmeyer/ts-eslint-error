# ts-eslint-error

A minimal reproduction of a ts-eslint-error.

In branch `local-and-action` the error is the same on local and super-linter. \
Now when running localy the error is because of a missing config, but the file `test.ts` is now included. \
But when looking at the action log, the file is still not included.

## Super-Linter

[![Lint Code Base](https://github.com/dominicmeyer/ts-eslint-error/actions/workflows/super-linter.yml/badge.svg)](https://github.com/dominicmeyer/ts-eslint-error/actions/workflows/super-linter.yml)

## Local

Seeing the error:

```sh
npm install
npx ts-standard
```

Output:

```text
ts-standard: Standard for TypeScript! (https://github.com/standard/ts-standard)
  /Users/meyerdom/Projekte/Privat/TsStandardError/test.ts:0:1: This rule requires the `strictNullChecks` compiler option to be turned on to function correctly. (@typescript-eslint/prefer-nullish-coalescing)
  /Users/meyerdom/Projekte/Privat/TsStandardError/test.ts:0:1: This rule requires the `strictNullChecks` compiler option to be turned on to function correctly. (@typescript-eslint/strict-boolean-expressions)
```
