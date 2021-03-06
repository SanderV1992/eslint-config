# Eslint Tests Configuration with Typescript Support

[![npm version](https://badge.fury.io/js/%40sanv%2Feslint-config-tests-typescript.svg)](https://badge.fury.io/js/%40sanv%2Feslint-config-tests-typescript)

1. Install the correct version of package, which are listed by the command:

```bash
npm install "@sanv/eslint-config-tests-typescript" --save-dev
```

2. Add next line to your `.eslintrc.js`:

```js
module.exports = {
  parser: '@typescript-eslint/parser',
  plugins: ['prettier', 'react', 'jsx-a11y', 'jest', '@typescript-eslint'],
  parserOptions: {
    project: './tsconfig.json',
    sourceType: 'module',
  },
  extends: [
    '@sanv/eslint-config-tests-typescript',
    'plugin:prettier/recommended',
    'prettier/react',
    'prettier/@typescript-eslint',
  ],
}
```
