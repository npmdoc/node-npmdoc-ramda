# npmdoc-ramda

#### api documentation for  [ramda (v0.23.0)](http://ramdajs.com/)  [![npm package](https://img.shields.io/npm/v/npmdoc-ramda.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-ramda) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-ramda.svg)](https://travis-ci.org/npmdoc/node-npmdoc-ramda)

#### A practical functional library for JavaScript programmers.

[![NPM](https://nodei.co/npm/ramda.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/ramda)

- [https://npmdoc.github.io/node-npmdoc-ramda/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-ramda/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ramda/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ramda/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-ramda/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-ramda/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Scott Sauyet",
        "url": "scott.sauyet.com"
    },
    "bugs": {
        "url": "https://github.com/ramda/ramda/issues"
    },
    "contributors": [
        {
            "name": "Michael Hurley",
            "url": "http://buzzdecafe.com"
        },
        {
            "name": "Scott Sauyet",
            "url": "http://fr.umio.us"
        },
        {
            "name": "David Chambers",
            "url": "http://davidchambers.me"
        },
        {
            "name": "Graeme Yeates",
            "url": "https://github.com/megawac"
        }
    ],
    "dependencies": {},
    "description": "A practical functional library for JavaScript programmers.",
    "devDependencies": {
        "acorn": "0.9.x",
        "benchmark": "~1.0.0",
        "browserify": "10.x.x",
        "cli-table": "0.3.x",
        "commander": "2.5.x",
        "dox": "latest",
        "envvar": "1.x.x",
        "escodegen": "1.4.x",
        "eslint": "^2.11.0",
        "handlebars": "3.0.x",
        "istanbul": "^0.4.x",
        "js-yaml": "^3.2.5",
        "jsverify": "^0.7.3",
        "mocha": "2.x.x",
        "q": "^1.1.1",
        "ramda": "0.17.x",
        "rimraf": "~2.3.2",
        "sanctuary": "0.7.x",
        "sinon": "^1.17.4",
        "testem": "0.9.x",
        "uglify-js": "2.4.x",
        "xyz": "1.0.x"
    },
    "directories": {},
    "dist": {
        "shasum": "ccd13fff73497a93974e3e86327bfd87bd6e8e2b",
        "tarball": "https://registry.npmjs.org/ramda/-/ramda-0.23.0.tgz"
    },
    "gitHead": "5dec606e0504af973cd6e0ceec8997b72800eb6b",
    "homepage": "http://ramdajs.com/",
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "aromano"
        },
        {
            "name": "buzzdecafe"
        },
        {
            "name": "crosseye"
        },
        {
            "name": "davidchambers"
        },
        {
            "name": "kedashoe"
        },
        {
            "name": "rane"
        },
        {
            "name": "scott-christopher"
        }
    ],
    "name": "ramda",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/ramda/ramda.git"
    },
    "scripts": {
        "bench": "scripts/benchRunner",
        "bookmarklet": "scripts/bookmarklet",
        "browser_test": "testem ci",
        "build": "make && make dist/ramda.min.js",
        "clean": "rimraf dist/* coverage/*",
        "coverage": "istanbul cover node_modules/.bin/_mocha -- --reporter spec",
        "lint": "eslint scripts/bookmarklet scripts/build src/*.js src/internal/*.js test/*.js test/**/*.js lib/sauce/*.js lib/bench/*.js",
        "postbrowser_test": "npm run posttest",
        "postcoverage": "npm run posttest",
        "posttest": "git checkout -- dist",
        "prebrowser_test": "npm run pretest",
        "precoverage": "npm run pretest",
        "test": "mocha --reporter spec"
    },
    "version": "0.23.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
