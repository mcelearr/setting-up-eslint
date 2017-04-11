# setting-up-eslint

1. Go [here](https://www.npmjs.com/package/eslint-config-airbnb) and follow the instructions.
2. Install the `linter`, `linter-eslint`, `linter-ui-default` atom packages.
3. Copy the `eslintrc.json` file in this repo into your repo's root directory.
4. `npm install --save-dev husky`.
5. Put the following scripts into your `package.json`
```json
  "prepush": "npm run lint",
  "lint": "./node_modules/.bin/eslint **.js"
```
6. If you are using node version manager, copy the below command into your terminal. I have used 6.10.1 here. Put whatever version of node your group's project is using.

```bash
touch .nvmrc & echo 6.10.1 >> .nvmrc
```
