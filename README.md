# Eslint-tools-m6web
The purpose of this package is simple, simplify the configuration of eslint and prettier in our projects.

It provides: 
- [eslint-config-m6web](https://github.com/M6Web/eslint-config-m6web) which inherits from [eslint-config-airbnb](https://github.com/airbnb/javascript)
- [eslint](https://eslint.org/) itself
- [prettier](https://github.com/prettier/prettier) with all the plugins needed to work with eslint

With that come some little changes from the default config of [eslint-config-airbnb](https://github.com/airbnb/javascript) and [prettier](https://github.com/prettier/prettier) that you can find in [.eslintrc](.eslintrc) file and [here](https://github.com/M6Web/eslint-config-m6web/blob/master/index.js).

## Setup

```shell
npm install eslint-tools-m6web
```

or 

```shell
yarn add eslint-tools-m6web
```

Then you need to inherit the config in the `.eslintrc` file of your project. For that create a `.eslintrc` and add the following lines:
```json
{
  "extends": "./node_modules/eslint-tools-m6web/.eslintrc"
}
```

And that's all.

If you want to customize some rules, follow the [eslint documentation](https://eslint.org/docs/user-guide/configuring). 

## USAGE
Lint your code:
```shell
yarn eslint src/
```

Rewrite your code, the right way :smiling_imp::
```shell
yarn prettier-eslint --write 'src/*.js'
```
