# ESLint Boilerplate Project

Basic boilerplate project for JavaScript and TypeScript Apps with ESLint and Prettier configuration. This project made based on Traversy Media tutorial about [VSCode ESLint, Prettier & Airbnb Style Guide Setup](https://www.youtube.com/watch?v=SydnKbGc7W8) and [ESLint Gist Setup](https://gist.github.com/bradtraversy/aab26d1e8983d9f8d79be1a9ca894ab4).

## Setup

This project using Yarn as package manager. But it can run with NPM too. For first setup, install Node JS in your device, and then run this script in to clone project with Git.

```sh
// Clone the repository
git clone -b master -o github --depth 1 --single-branch https://github.com/javascript-indonesias/ESLintBoilerplates.git
```

Run script inside project to install needed dependencies.

```sh
yarn install
```

or using NPM

```sh
npm install
```

## Setup Default Formatter and Autofix On Save

Install [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) and [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) plugin from VS Code Marketplace, and add this snippets in your VS Code Settings "settings.json" file.

```sh
    "editor.formatOnSave": true,
    "[javascript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[typescript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "editor.codeActionsOnSave": {
        "source.fixAll.eslint": true
    }
```

Those snippet add ability to auto format your JavaScript code and autofixing it if there are ESLint error. You can freely change this setting as your needs. You can follow the issue about [ESLint settings here](https://github.com/microsoft/vscode-eslint/issues/833).

## Customization

Some rules and ESLint parser can be edited in **eslintrc.json** file. If you're working with JavaScript projects, you can disable TypeScript parser in eslintrc file. Or if you working with TypeScript projects, you can activate rule and parser for TypeScript linting. For complete ESLint Rules reference, check in [https://eslint.org/docs/rules/](https://eslint.org/docs/rules/).
