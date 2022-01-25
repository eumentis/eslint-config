# ESLint config for React apps

This package provides a sharable ESLint config used by [Eumentis](https://eumentis.com) for React apps

### Features

- Uses Airbnb's ESLint config
- Supports Typescript linting along with type checking rules
- Supports React 17+
- Uses latest versions of ESLint & TypeScript ESLint

## Install

Using NPM

```bash
npm install --save-dev @eumentis/eslint-config
```

Using Yarn

```bash
yarn add -D @eumentis/eslint-config
```

## Usage

Add the following to your ESLint config file

```javascript
{
  extends: ['@eumentis'],
  parserOptions: {
    project: './tsconfig.json'
  }
}
```

Type checking is enabled by default in this config. Therefore, you will need to create a `tsconfig.json` file in your project root.
