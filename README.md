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

## How to Resolve ESLint Plugin Conflicts in Create react app setup (Optional)

If you encounter an ESLint conflict error `[eslint] Plugin "react" was conflicted between ".eslintrc.js` in a project created using 'create-react-app', follow these steps:

1. Create a .env file in your project's root directory.(if not present)
2. Add the following line to the .env file:

```shell
DISABLE_ESLINT_PLUGIN=true
```

Here we are disabling the default ESLint configuration in a 'Create React App' project and using our custom configuration instead, which can be helpful for finding linting error during development.

