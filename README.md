# TSConfigs

A collection of TSConfigs to extend in your own apps, tuned to a particular runtime environment.

[![NPM Version][version_badge]][npm_url]
[![NPM Downloads][downloads_badge]][npm_url]

- [TSConfigs](#tsconfigs)
  - [Install](#install)
  - [Available Configurations](#available-configurations)
  - [License](#license)

## Install

```sh
# NPM
npm add --save-dev @giotramu/tsc typescript

# PNPM
pnpm add --save-dev @giotramu/tsc typescript

# Yarn
yarn add --dev @giotramu/tsc typescript
```

## Available Configurations

<details>

<summary><strong>Node.js - CJS</strong></summary>

> ⚠️ The following configuration supports a version of Node >= 16.

Add to your `tsconfig.json`:

```json
{
  "extends": "@giotramu/tsc/node/tsconfig.cjs.json",
  "compilerOptions": {
    "declarationDir": "./types",
    "typeRoots": ["./types", "./node_modules/@types"]
  }
}
```
</details>

<details>

<summary><strong>Node.js - ESM</strong></summary>

> ⚠️ The following configuration supports a version of Node >= 16.

Add to your `tsconfig.json`:

```json
{
  "extends": "@giotramu/tsc/node/tsconfig.esm.json",
  "compilerOptions": {
    "declarationDir": "./types",
    "typeRoots": ["./types", "./node_modules/@types"]
  }
}
```
</details>

<details>

<summary><strong>React.js</strong></summary>

> ⚠️ The following configuration is helpful in projects based on Create React App and Next.js.

Add to your `tsconfig.json`:

```json
{
  "extends": "@giotramu/tsc/react/tsconfig.json"
}
```
</details>

## License

[MIT License](./LICENSE)

<!-- Badges -->
[downloads_badge]: https://img.shields.io/npm/dm/@giotramu/tsc?style=flat-square&colorA=313133&colorB=4169E1
[version_badge]: https://img.shields.io/npm/v/@giotramu/tsc?style=flat-square&colorA=313133&colorB=4169E1

<!-- Links -->

[npm_url]: https://www.npmjs.com/package/@giotramu/tsc
