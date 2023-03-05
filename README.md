# TypeScript

```sh
# NPM
npm add --save-dev typescript @giotramu/tsc

# PNPM
pnpm add --save-dev typescript @giotramu/tsc

# Yarn
yarn add --dev typescript @giotramu/tsc
```

Dopo aver installato il pacchetto, è possibile estendere la configurazione base di TypeScript utilizzando il file `tsconfig.json`, solitamente posizionato all'interno della root di progetto. Al momento sono supportati solo due tipi di _environment_:

- [Node](#node)
- [React](#react)

## Node

Questa configurazione TypeScript supporta una versione di Node >= 14.

```json
{
  "extends": "@giotramu/tsc/node/tsconfig.json",
  "compilerOptions": {
    "declarationDir": "./types",
    "typeRoots": ["./types", "./node_modules/@types"]
  }
}
```

## React

Questa configurazione supporta anche progetti basati su Create React App e Next.js.

```json
{
  "extends": "@giotramu/tsc/tsconfig.react.json"
}
```
