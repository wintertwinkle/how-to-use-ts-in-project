# About

This is a project amis to teach myself how to use typescirpt in project.

## How to use `TypeScript`

1. Initializing the Project

   ```bash
   npm init -y
   ```

2. Install the TypeScript Compiler

   ```bash
   npm install -D typescript
   ```

3. configure `tsconfig.json`

   ```json
   {
     "compilerOptions": {
       "module": "commonjs",
       "esModuleInterop": true,
       "target": "es6",
       "moduleResolution": "node",
       "sourceMap": true,
       "outDir": "dist"
     },
     "lib": ["es2015"]
   }
   ```

   JSON snippet explanation:

   - `module`: Specifies the module code generation method. Node uses commonjs.
   - `target`: Specifies the output language level.
   - `moduleResolution`: This helps the compiler figure out what an import refers to. The value node mimics the module resolution mechanism.
   - `outDir`: This is the location to output .js files after transpilation.

   More information about configration: [Typescript documentation](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html)

## How to use `eslint`

1. install `eslint` using `npm`

   ```bash
   npm install --save-dev eslint
   ```

2. run `eslint` initialization command

   ```bash
   npx eslint --init
   ```

This will ask you a series of questions:

- How would you like to use `ESlint`?
- What type of modules does your project use?
- which framework does your project use?
- Does your project use TypeScript?
- Where does your code run?
- What format do you want your config file to be in?

After that, you will be prompted to install some additional eslint libraries.

Finally, you'll get a configuration file: `eslintrc.js`(which is based on your answer to questions of 'What format do you want your config file to be in?')

## Resouce

[Tutorial](https://www.digitalocean.com/community/tutorials/setting-up-a-node-project-with-typescript)
