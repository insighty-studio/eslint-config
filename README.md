# insighty-eslint-config
Standard Insighty ESLint configuration.

## How do I use this?
### Getting Started
1. Pick one of the included configs
1. Copy to the root of your project, right next to your `package.json`
1. Install dependencies as described below
## Included configs

### [Basic ES6](es6-basic/.eslintrc.json)
Dependencies:
`yarn add --dev eslint babel-eslint eslint-config-airbnb-base eslint-plugin-import`

### [React](react/.eslintrc.json)
Dependencies:
`yarn add --dev eslint babel-eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react`

### Common Usage Patterns

#### Scripts
For the sake of simplicity, it is recommended to extend the `package.json` `"scripts"` section with the following:
```
    "lint": "eslint .",
    "lint-fix": "eslint . --fix",
```
[What is `--fix`?](https://eslint.org/docs/user-guide/command-line-interface#--fix)

#### Running on the CI server
Then, linting can be plugged into the CI build or git's [`pre-commit`](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks) hook via `yarn lint` or `npm run lint`

## Have an RFC? Having Troubles?
Please open a GitHub issue or submit a pull request.
