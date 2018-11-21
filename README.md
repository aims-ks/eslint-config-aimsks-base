# eslint-config-aimsks-base

This package provides the AIMS Knowledge Systems teams base ESLint configuration for Javascript 
projects. This package essentially provides overrides to the Airbnb **eslint-config-airbnb-base**
package to meet AIMS Knowledge Systems style guidelines.

## Usage

Step 1. Add the following to the `dev-dependencies` in `package.json`.

```
  "eslint": "^4.19.1",
  "eslint-plugin-import": "^2.14.0",
  "eslint-config-aimsks-base": "git+https://github.com/aims-ks/eslint-config-aimsks-base.git",
```

Step 2. Add an `.eslintrc` file to the root of the project directory with the contents:

```
{
  "root": true,
  "parserOptions": {
    "ecmaVersion": 2017,
    "sourceType": "module"
  },
  "extends": "aimsks-base",
  "env": {
    "browser": true,
    "node": true,
    "es6": true,
    "mocha": true,
    "amd": true
  },
  "rules": {

    // Project specific overrides. This is discouraged.

  }
}
```