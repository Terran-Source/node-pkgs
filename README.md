# node-pkgs
Holds all the public Node packages (npm) for `@terran-source`

## How to use any of these packages

Create an _.npmrc_ file inside the same folder as _package.json_ (if it's not already there).
```bash
  my-project
  |- package.json
  |- .npmrc // ☚ 
  |- ... (others)
```
Then, add the following line inside _.npmrc_:
#### If it's public package
```
@terran-source:registry=https://npm.pkg.github.com/
always-auth=false
```
#### If it's private package
```
//npm.pkg.github.com/:_authToken=${NODE_AUTH_TOKEN}
@terran-source:registry=https://npm.pkg.github.com/
always-auth=true
```

Now, add the package as dependency to your project

#### via `npm`

`npm install @terran-source/hooks`

#### via `yarn`

`yarn add @terran-source/hooks`
