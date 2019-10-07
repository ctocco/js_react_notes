# ESlint setup

1. npm install -D eslint eslint-config-prettier
2. now make this file here in your root folder .eslintrc.json
3. in scripts in your package.json write

```js
 "lint": "eslint \"src/\**/*.{js, jsx}\" --quiet",
```

4. npm run lint
5. also if you have VS studio code you can install this in your editor
