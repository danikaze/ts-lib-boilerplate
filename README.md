# ts-lib-boilerplate

A boilerplate to to create npm/libraries based on TypeScript

## Features

### Ready
- TypeScript support with path aliases
- [Linting](https://palantir.github.io/tslint/)

### Planned

- [Prettier](https://prettier.io/)
- [Git hooks](https://github.com/typicode/husky)
- Migrate to [typescript-eslint](https://github.com/typescript-eslint/typescript-eslint)
- Unit testing

## Development

Creating libraries with this boilerplate should be easy.

```
npm run dev
```

Executes a `webpack --watch` command, outputting the files into the `dist` folder

```
npm run build
```

Runs the linter and the tests if any. If these checks pass, builds the library into the `dist` folder and asks if the package should be published or not.

`npm run build -- --only` (or `./scripts/build.sh --only`) executes the building process without any checks, and also doesn't ask for publishing. Might be useful to quickly test the production output.

```
npm run clean
```

Will remove the `dist` repository. It's executed automatically before building to avoid leaving any unwanted file.
