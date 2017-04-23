# npmdoc-rbush

#### api documentation for  [rbush (v2.0.1)](https://github.com/mourner/rbush)  [![npm package](https://img.shields.io/npm/v/npmdoc-rbush.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-rbush) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-rbush.svg)](https://travis-ci.org/npmdoc/node-npmdoc-rbush)

#### High-performance 2D spatial index for rectangles (based on R*-tree with bulk loading and bulk insertion algorithms)

[![NPM](https://nodei.co/npm/rbush.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/rbush)

- [https://npmdoc.github.io/node-npmdoc-rbush/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-rbush/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-rbush/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-rbush/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-rbush/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-rbush/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Vladimir Agafonkin"
    },
    "bugs": {
        "url": "https://github.com/mourner/rbush/issues"
    },
    "dependencies": {
        "quickselect": "^1.0.0"
    },
    "description": "High-performance 2D spatial index for rectangles (based on R*-tree with bulk loading and bulk insertion algorithms)",
    "devDependencies": {
        "benchmark": "^2.1.0",
        "browserify": "^13.0.1",
        "eslint": "^2.10.2",
        "eslint-config-mourner": "^2.0.1",
        "faucet": "0.0.1",
        "istanbul": "~0.4.3",
        "tape": "^4.5.1",
        "uglify-js": "^2.6.4"
    },
    "directories": {},
    "dist": {
        "shasum": "4cfaca28c3064bc0ee75431a1b79990e875eefa9",
        "tarball": "https://registry.npmjs.org/rbush/-/rbush-2.0.1.tgz"
    },
    "eslintConfig": {
        "extends": "mourner",
        "rules": {
            "new-cap": 0,
            "consistent-return": 0
        }
    },
    "gitHead": "86fb9f11f45a36ee96d1e80b26fd51bcf7310d7b",
    "homepage": "https://github.com/mourner/rbush",
    "keywords": [
        "spatial",
        "tree",
        "search",
        "rectangle",
        "index",
        "math"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "mourner"
        }
    ],
    "name": "rbush",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/mourner/rbush.git"
    },
    "scripts": {
        "build": "browserify index.js -s rbush -o rbush.js",
        "build-min": "browserify index.js -s rbush | uglifyjs -c warnings=false -m > rbush.min.js",
        "cov": "istanbul cover test/test.js -x test/test.js",
        "perf": "node ./debug/perf.js",
        "prepublish": "npm run build && npm run build-min",
        "test": "eslint index.js test/test.js && node test/test.js | faucet"
    },
    "version": "2.0.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
