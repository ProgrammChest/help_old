# Babel

package.json

```json
{
  "name": "NAME",
  "version": "0.0.0",
  "private": true,
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "build": "rimraf dist && nodemon bin/server.js --exec babel-node",
    "start": "npm run build && node bin/server.js"
  },
  "dependencies": {
    "@babel/runtime": "^7.9.6",
  },
  "devDependencies": {
    "@babel/cli": "^7.8.4",
    "@babel/core": "^7.9.6",
    "@babel/node": "^7.8.7",
    "@babel/plugin-transform-runtime": "^7.9.6",
    "@babel/plugin-transform-typescript": "^7.9.6",
    "@babel/preset-env": "^7.9.6",
    "@babel/preset-typescript": "^7.9.0"
  }
}
```

.babelrc

```json
{
    "presets": [
        "@babel/preset-env",
        "@babel/preset-typescript"
    ],
    "ignore": [
        "./node_modules",
        "./.babelrc",
        "./npm-debug.log"
    ],
    "plugins": ["@babel/plugin-transform-runtime", "@babel/plugin-transform-typescript"]
}
```
