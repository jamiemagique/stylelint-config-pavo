# Pavo stylelint config

[![Greenkeeper badge](https://badges.greenkeeper.io/jamiemagique/stylelint-config-pavo.svg)](https://greenkeeper.io/)
![Status](https://david-dm.org/jamiemagique/stylelint-config-pavo.svg)

Linting and Formatting with Prettier.

## 1. Install

```
npm install stylelint-config-pavo --save-dev
```

## 2. Usage

Create a `.stylelintrc` file.

Add this configuration to extend:

```
{
  "extends": "stylelint-config-pavo"
  "rules": {
    // Your projects overrides.
  }
}
```

You can layer multiple configurations depending upon your projects type:

```
{
  "extends": ["stylelint-config-pavo", "stylelint-config-pavo/<config-name>"]
}
```

Additional configs available are:

* styled-components

## Prettier integration

### Visual Studio Code

Sample `.vscode/settings.json` config:

```
{
  "editor.trimAutoWhitespace": true,
  "stylelint.enable": true,
  "prettier.tabWidth": 2,
  "prettier.trailingComma": "all",
  "prettier.bracketSpacing": true,
  "prettier.singleQuote": true,
  "prettier.stylelintIntegration": true,
  "prettier.semi": true,
  "prettier.useTabs": false,
  "prettier.printWidth": 160,
  "files.trimTrailingWhitespace": true
}
```
