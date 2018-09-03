# Rxjs-exercises
Test project based on Node.JS, without any framework but RxJS. Project is created for TypeScript. TSLint is also configured.

## How to use
yarn run watch - run typescript compiler in watch mode, so any changes make recompilation

yarn run start - run the application

yarn run lint - run tslint

## debugging with VS Code
In the main catalog create folder .vscode and file launch.json:  .vscode/launch.json
Paste followed code into launch.json:
```
{
  // Use IntelliSense to learn about possible attributes.
  // Hover to view descriptions of existing attributes.
  // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
  "version": "0.2.0",
  "configurations": [{
    "type": "node",
    "request": "launch",
    "name": "Launch Program",
    "program": "${workspaceFolder}/src/index.ts",
    "preLaunchTask": "tsc: build - tsconfig.json",
    "outFiles": [
      "${workspaceFolder}/dist/**/*.js"
    ],
    "env": {
      "NODE_PATH": "dist"
    }
  }]
}
```
