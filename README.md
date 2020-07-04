# cra-template-optimized

This is an optimized typescript template for [Create React App](https://github.com/facebook/create-react-app).

It generates an app that follows the file structure described [here](https://medium.com/@Charles_Stover/optimal-file-structure-for-react-applications-f3e35ad0a145)

```
my-app
├── build
├── node_modules
├── public
│   ├── favicon.ico
│   ├── index.html
│   └── manifest.json
├── src
│    ├── components
│    │   ├── component-name
│    │   │   ├── component-name.css
│    │   │   ├── component-name.scss
│    │   │   ├── component-name-styles.tsx
│    │   │   ├── component-name.tsx
│    │   │   └── index.ts
│    │   └── index.ts
│    ├── images
│    │   │   └── logo.svg
│    ├── packages
│    │   └── ...
│    ├── utils
│    │   ├── ...
│    │   └── index.ts
│    ├── index.css
│    ├── index.tsx
│    └── service-worker.ts
├── .gitignore
├── package.json
└── README.md
```

## Usage
```shell script
yarn create react-app my-app --template @es50678/optimized-ts
```

## make sure you have added the scope to your npm user

Detailed instructions can be found [here](https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line). 

When creating the token:
* Name the token `@es50678 scope Package Registry Access` (or something similarly descriptive).
* Select:
  * `write:packages`
  * `read:packages`
  * All `repo` scopes (this should get done automatically).

> Ensure you copy the token down, you will need it later.

## npm/yarn

```
$ npm login --registry=https://npm.pkg.github.com --scope=@es50678
> Username: GITHUB_USERNAME
> Password: TOKEN
> Email: GITHUB_EMAIL_ADDRESS
```

For more information, please refer to:

- [Getting Started](https://create-react-app.dev/docs/getting-started) – How to create a new app.
- [User Guide](https://create-react-app.dev) – How to develop apps bootstrapped with Create React App.
