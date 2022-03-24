# About

This is a project amis to teach myself how to use typescirpt in project.

## Steps

1. In Initializing the Project

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
   - `outDir`: This is the location to output .js files after transpilation. In this tutorial you will save it as dist.

   More information about configration: [Typescript documentation](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html)

## Resouce

[Tutorial](https://www.digitalocean.com/community/tutorials/setting-up-a-node-project-with-typescript)
