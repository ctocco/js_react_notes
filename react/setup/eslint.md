# ESlint setup

1. npm install -D eslint eslint-config-prettier
2. now make this file here in your root folder .eslintrc.json
3. in scripts in your package.json write

```js
 "lint": "eslint \"src/\**/*.{js, jsx}\" --quiet",
```

4. npm run lint
5. also if you have VS studio code you can install this in your editor
6. npm install -D babel-eslint eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react

- the above is so that eslint works with react and jsx and it understands react correctly
- babel is the transpiler which doesn't understand react so well

7. go to eslint file under "eslint: recommended" and type in the following below

"plugin:import/errors",
"plugin:react/recommended",
"plugin:jsx-a11y/recommended"

8. plugins: ["react", "import", "jsx-a11y"]
9. "rules" : {
   "react/prop-types":0,
   "no-console": 1
   }

- no console won't give you a warning for console log
- prop types not neccessary with type script
- 0 means off and 1 means on

please see the file which you can copy into your project
