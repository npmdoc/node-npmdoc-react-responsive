# npmdoc-react-responsive

#### api documentation for  [react-responsive (v1.2.10)](http://github.com/contra/react-responsive)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-responsive.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-responsive) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-responsive.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-responsive)

#### Media queries in react for responsive design

[![NPM](https://nodei.co/npm/react-responsive.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-responsive)

- [https://npmdoc.github.io/node-npmdoc-react-responsive/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-responsive/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-responsive/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-responsive/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-responsive/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-responsive/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "react-responsive",
    "description": "Media queries in react for responsive design",
    "version": "1.2.10",
    "homepage": "http://github.com/contra/react-responsive",
    "repository": {
        "type": "git",
        "url": "git://github.com/contra/react-responsive.git"
    },
    "author": "Contra <yo@contra.io> (http://contra.io)",
    "license": "MIT",
    "main": "./dist/react-responsive.js",
    "files": [
        "dist"
    ],
    "keywords": [
        "css",
        "react-component",
        "viewport",
        "react",
        "mobile",
        "media queries",
        "respond",
        "media query",
        "matchMedia",
        "responsive",
        "component"
    ],
    "dependencies": {
        "hyphenate-style-name": "^1.0.0",
        "matchmedia": "^0.1.2",
        "prop-types": "^15.5.7"
    },
    "peerDependencies": {
        "react": "*"
    },
    "devDependencies": {
        "babel-cli": "^6.18.0",
        "babel-core": "^6.18.0",
        "babel-eslint": "^7.1.0",
        "babel-loader": "^6.2.7",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-transform-runtime": "^6.15.0",
        "babel-preset-es2015": "^6.18.0",
        "babel-preset-es2015-loose": "^8.0.0",
        "babel-preset-react": "^6.16.0",
        "babel-preset-stage-0": "^6.16.0",
        "babel-register": "^6.18.0",
        "chai": "^3.5.0",
        "eslint": "^3.9.0",
        "eslint-config-rackt": "^1.1.1",
        "github-changes": "^1.0.4",
        "jsdom": "^8.4.0",
        "mocha": "^2.4.5",
        "react": "^15.0.1",
        "react-addons-test-utils": "^15.0.1",
        "react-dom": "^0.14.0 || ^15.0.0",
        "should": "^8.0.2",
        "sinon": "^1.17.3",
        "webpack": "^1.13.3",
        "webpack-dev-server": "^1.16.2"
    },
    "scripts": {
        "preversion": "npm run clean && npm run build && npm docs",
        "postversion": "npm run changelog",
        "start": "$(npm bin)/webpack-dev-server --config webpack.config.samples.js  --content-base samples/sandbox/src --host 0.0.0.0 --hot --inline --port 3333",
        "build": "$(npm bin)/webpack",
        "build:watch": "npm run build -- --watch",
        "clean": "rimraf dist",
        "lint": "$(npm bin)/eslint src",
        "test": "NODE_PATH=$NODE_PATH:$PWD/src $(npm bin)/mocha -R spec --compilers js:babel-register --require ./test/setup.js test/*_test.js",
        "changelog": "github-changes -o contra -r react-responsive -b master -f ./CHANGELOG.md --order-semver --use-commit-body",
        "docs": "npm run docs:pre && npm run docs:build && npm run docs:publish",
        "docs:pre": "gitbook install && rimraf _book",
        "docs:build": "gitbook build -g contra/react-responsive",
        "docs:publish": "cd _book && git init && git commit --allow-empty -m 'update book' && git checkout -b gh-pages && touch .nojekyll && git add . && git commit -am 'update book' && git push git@github.com:contra/react-responsive gh-pages --force"
    },
    "babel": {
        "presets": [
            "es2015",
            "react",
            "stage-0"
        ],
        "plugins": [
            "add-module-exports"
        ]
    },
    "eslintConfig": {
        "parser": "babel-eslint",
        "extends": "rackt",
        "env": {
            "browser": true,
            "node": true,
            "es6": true
        },
        "ecmaFeatures": {
            "modules": true
        },
        "rules": {
            "semi": [
                2,
                "never"
            ]
        }
    },
    "engines": {
        "node": ">= 0.10"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
