# constructions 

1. run `npm init`
    - init `package.json` file.

1. run `npm install --save-dev @babel/core @babel/cli`
    - install babel.

1. run `npm install --save-dev @babel/preset-env`
    - @babel/priset-env transpile es6 to es5

1. run `touch .babelrc` and run `vi .babelrc`.
    ```
    const presets =  [
      ["@babel/preset-env"]
    ];

    module.exports = { presets }
    ```

1. run `mkdir src build`
    - add dir for build.

1. run `vi package.json`, and add npm command "build".
    - `--source-maps` option: create source-map file on build.
    ```
    {
        "scripts":{
            "build": "babel src -d build --source-maps"
        }
    }
    ```
    
1. run `touch src/index.js` and run `vi src/index.js`
    - create your source code.


# build
```
npm run build
```


