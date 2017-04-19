# npmtest-baobab

#### test coverage for  [baobab (v2.4.3)](https://github.com/Yomguithereal/baobab)  [![npm package](https://img.shields.io/npm/v/npmtest-baobab.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-baobab) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-baobab.svg)](https://travis-ci.org/npmtest/node-npmtest-baobab)

#### JavaScript persistent data tree with cursors.

[![NPM](https://nodei.co/npm/baobab.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/baobab)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-baobab/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-baobab/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-baobab/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-baobab/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-baobab/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-baobab/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-baobab/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-baobab/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-baobab/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-baobab/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-baobab/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-baobab/build/test-report.html](https://npmtest.github.io/node-npmtest-baobab/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-baobab/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-baobab/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-baobab/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-baobab/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-baobab/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-baobab/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-baobab/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-baobab/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Guillaume Plique",
        "url": "http://github.com/Yomguithereal"
    },
    "bugs": {
        "url": "https://github.com/Yomguithereal/baobab/issues"
    },
    "dependencies": {
        "emmett": "^3.1.1"
    },
    "description": "JavaScript persistent data tree with cursors.",
    "devDependencies": {
        "@yomguithereal/eslint-config": "^1.1.1",
        "add-banner": "^0.1.0",
        "async": "^1.2.1",
        "babel": "^5.6.14",
        "babelify": "^6.1.2",
        "benchmark": "^1.0.0",
        "browserify": "^12.0.1",
        "eslint": "^1.1.0",
        "lodash": "^3.6.0",
        "mkdirp": "^0.5.1",
        "mocha": "^2.0.1",
        "uglify-js": "^2.6.1"
    },
    "directories": {},
    "dist": {
        "shasum": "9655d6f1a69ce66a82fc6391773ca6a9f7a25a9d",
        "tarball": "https://registry.npmjs.org/baobab/-/baobab-2.4.3.tgz"
    },
    "gitHead": "4833e50a6cd64dc2c8bff655a319ede7041df836",
    "homepage": "https://github.com/Yomguithereal/baobab",
    "keywords": [
        "cursors",
        "atom",
        "tree",
        "react"
    ],
    "license": "MIT",
    "main": "./dist/baobab.js",
    "maintainers": [
        {
            "name": "yomguithereal"
        }
    ],
    "name": "baobab",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/Yomguithereal/baobab.git"
    },
    "scripts": {
        "benchmark": "babel-node benchmark.js",
        "build": "mkdirp build && browserify ./src/baobab.js -t [babelify --loose all] -s Baobab -o ./build/baobab.js && uglifyjs ./build/baobab.js -c -m -o ./build/baobab.min.js && node ./scripts/banner.js",
        "check": "npm test && npm run lint && npm run build",
        "dist": "babel ./src --out-dir dist",
        "lint": "eslint -c eslint.config.js ./src ./test",
        "prepublish": "npm run dist",
        "test": "mocha -R spec --compilers js:babel/register ./test/endpoint.js"
    },
    "version": "2.4.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
