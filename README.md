# @vancats/eslint-config


[![npm](https://img.shields.io/npm/v/@vancats/eslint-config?color=a1b858&label=)](https://npmjs.com/package/@vancats/eslint-config)

## Usage

### Install

```bash
# for all-sided
pnpm add -D eslint @vancats/eslint-config
# for javascript
pnpm add -D eslint @vancats/eslint-config-basic
# for typescript
pnpm add -D eslint @vancats/eslint-config-ts
# for react + ts
pnpm add -D eslint @vancats/eslint-config-react
# for vue + ts
pnpm add -D eslint @vancats/eslint-config-vue
```

### Config `.eslintrc`

```json
{
  "extends": "@vancats"
}
// or
{
  "extents": "@vancats/eslint-config-ts"
}
```

### Add script for package.json

For example:

```json
{
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "eslint . --fix"
  }
}
```

### Config VSCode auto fix

Create `.vscode/settings.json`

```json
{
  "prettier.enable": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```
