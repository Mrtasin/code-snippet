# Prettier Configuration Guide

This document contains some available Prettier configuration options with their descriptions.

## Installation

```bash
npm install --save-dev prettier
```

## Basic Usage

```bash
npx prettier --write .
```

---
- Create a file .prettierrc 

## `.prettierrc` Example

```json
{
  "tabWidth": 2,
  "useTabs": false,
  "semi": true,
  "singleQuote": false,
  "trailingComma": "all",
  "bracketSpacing": true,
  "arrowParens": "always"
}
```

---

## All Configuration Options

| Option                       | Type      | Description |
|-----------------------------|-----------|-------------|
| `tabWidth`                  | number    | Number of spaces per tab. Default is `2`. |
| `useTabs`                   | boolean   | Indent with tabs instead of spaces. |
| `semi`                      | boolean   | Add semicolons at the ends of statements. |
| `singleQuote`               | boolean   | Use single quotes instead of double quotes. |
| `trailingComma`             | string    | Print trailing commas wherever possible. Values: `"none"`, `"es5"`, `"all"`. |
| `bracketSpacing`            | boolean   | Print spaces between brackets in object literals. |
| `arrowParens`               | string    | Include parentheses around a sole arrow function parameter. Values: `"avoid"`, `"always"`. |

---

## Ignore Files

- Create another file .prettierignore
- 
Use `.prettierignore` to exclude files:

```
node_modules
dist
build
.env
```

---

## Scripts in `package.json`

```json
"scripts": {
  "format": "prettier --write .",
}
```


## Run command

```bash
npm run format
```
