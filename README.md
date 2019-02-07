# Atom Space ESLint Preset

`@atomspace/eslint` is a Neutrino preset that supports linting JavaScript projects with ESLint config used in Atom Space.

## Features

- Zero upfront configuration necessary to start linting your project
- Modern Babel knowledge supporting ES modules, JSX (when used - with React preset), Web and Node.js apps
- Highly visible during development, fails compilation when - building for production
- Promises linting
- Module systems linting (ES, CommonJS, AMD)
- Regex shorthand to improve readability
- ESLint comments linting
- JSDoc syntax linting
- Easily extensible to customize your project as needed

``` ❯ npm install --save-dev neutrino "@atomspace/eslint" ```

## Project layout

`@atomspace/eslint` follows the standard [project layout](readme.md)  specified by Neutrino. This means that by default all project source code should live in a directory named src in the root of the project.

## Quick start

### .neutrinorc.js

```js
module.exports = {
   use: [
      '@atomspace/eslint'

      // put your rest of presets here
   ]
};
```
### .neutrinorc.js

```json
{
   "scripts": {
      "start": "neutrino start",
      "build": "neutrino build",
      "lint": "neutrino lint"
   }
}
```



 Name | Description | Environments and Commands
---------|----------|---------
 `lint` | Lints JS and JSX files from the `src` directory using ESLint. Contains a single loader named eslint. This is inherited from @neutrinojs/eslint. | all

 `@atomspace/eslint` can work in your editor even if there is no build infrastructure (`npm start` / `npm run build`). You can install it to any kind of JavaScript projects following the [ESLint CLI](#eslint-cli) guide above.`
