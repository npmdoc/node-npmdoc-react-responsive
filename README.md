# api documentation for  [react-responsive (v1.2.7)](http://github.com/contra/react-responsive)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-responsive.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-responsive) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-responsive.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-responsive)
#### Media queries in react for responsive design

[![NPM](https://nodei.co/npm/react-responsive.png?downloads=true)](https://www.npmjs.com/package/react-responsive)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-responsive/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-react-responsive_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-responsive/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-responsive/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-responsive/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Contra",
        "email": "yo@contra.io",
        "url": "http://contra.io"
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
    "bugs": {
        "url": "https://github.com/contra/react-responsive/issues"
    },
    "dependencies": {
        "hyphenate-style-name": "^1.0.0",
        "matchmedia": "^0.1.2"
    },
    "description": "Media queries in react for responsive design",
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
    "directories": {},
    "dist": {
        "shasum": "c6fa23f7a28652d04dbf4d10e60ddbd46fc191a5",
        "tarball": "https://registry.npmjs.org/react-responsive/-/react-responsive-1.2.7.tgz"
    },
    "engines": {
        "node": ">= 0.10"
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
    "files": [
        "dist"
    ],
    "gitHead": "ee6b1429caa0fefd6e6f7c9313fe54fe13a61d82",
    "homepage": "http://github.com/contra/react-responsive",
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
    "license": "MIT",
    "main": "./dist/react-responsive.js",
    "maintainers": [
        {
            "name": "contra",
            "email": "contra@wearefractal.com"
        },
        {
            "name": "fractal",
            "email": "contact@wearefractal.com"
        }
    ],
    "name": "react-responsive",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "*"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/contra/react-responsive.git"
    },
    "scripts": {
        "build": "$(npm bin)/webpack",
        "build:watch": "npm run build -- --watch",
        "changelog": "github-changes -o contra -r react-responsive -b master -f ./CHANGELOG.md --order-semver --use-commit-body",
        "clean": "rimraf dist",
        "docs": "npm run docs:pre && npm run docs:build && npm run docs:publish",
        "docs:build": "gitbook build -g contra/react-responsive",
        "docs:pre": "gitbook install && rimraf _book",
        "docs:publish": "cd _book && git init && git commit --allow-empty -m 'update book' && git checkout -b gh-pages && touch .nojekyll && git add . && git commit -am 'update book' && git push git@github.com:contra/react-responsive gh-pages --force",
        "lint": "$(npm bin)/eslint src",
        "postversion": "npm run changelog",
        "preversion": "npm run clean && npm run build && npm docs",
        "start": "$(npm bin)/webpack-dev-server --config webpack.config.samples.js  --content-base samples/sandbox/src --host 0.0.0.0 --hot --inline --port 3333",
        "test": "NODE_PATH=$NODE_PATH:$PWD/src $(npm bin)/mocha -R spec --compilers js:babel-register --require ./test/setup.js test/*_test.js"
    },
    "version": "1.2.7"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module react-responsive](#apidoc.module.react-responsive)
1.  object <span class="apidocSignatureSpan">react-responsive.</span>defaultProps
1.  string <span class="apidocSignatureSpan">react-responsive.</span>displayName



# <a name="apidoc.module.react-responsive"></a>[module react-responsive](#apidoc.module.react-responsive)



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
