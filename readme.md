# ESLint and Prettier Setup (VS Code)

## What it does 
- JS Linting based on latest standard
-Fixes formatting issue and error with Prettier
- Lint fixes React via eslint-config-airbnb

## How to install

### Local Project Install Method

1.) if project doesnt have a `package.json` file, create one with `npm init`

2.) Run the following command to install setup and install peerDependencies as devDependencies on current project. 

`npx install-peerdeps --dev @dg-sbae/eslint-config`

3.) Create a `eslintrc` file in the root of your project's directory and add this:
```
{
  "extends": [
   "@dg-sbae/eslint-config"
   
  ]
}
```

### Global Install

2.) Make a global `.eslintrc` file

ESLint will look for one in your home directory

`~/.eslintrc` for mac
`C:\Users\username\.eslintrc` for windows
In your `.eslintrc` file, it should look like this:
```
{
  "extends": [
    "@dg-sbae/eslint-config"
  ]
}
```