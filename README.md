# npm-pkgs
Holds all the public Node packages (npm) for `@Terran-Source`

## How to use any of these packages

Create an _.npmrc_ file inside the same folder as _package.json_ (if it's not already there).
```bash
  my-project
  |- package.json
  |- .npmrc // ☚ 
  |- ... (others)
```
Then, add the following line inside _.npmrc_:
```
@Terran-Source:registry=https://npm.pkg.github.com
```

Now, add the package as dependency to your project

#### via `npm`

`npm install @Terran-Source/hooks`

#### via `yarn`

`yarn add @Terran-Source/hooks`
