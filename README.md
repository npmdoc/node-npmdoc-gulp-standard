# npmdoc-gulp-standard

#### api documentation for  [gulp-standard (v10.0.0)](https://github.com/emgeee/gulp-standard)  [![npm package](https://img.shields.io/npm/v/npmdoc-gulp-standard.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gulp-standard) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-standard.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-standard)

#### gulp plugin for checking JavaScript code with the standard syntax

[![NPM](https://nodei.co/npm/gulp-standard.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/gulp-standard)

- [https://npmdoc.github.io/node-npmdoc-gulp-standard/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-gulp-standard/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-standard/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-standard/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gulp-standard/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gulp-standard/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matt Green",
        "url": "http://emgeee.com/"
    },
    "bugs": {
        "url": "https://github.com/emgeee/gulp-standard/issues"
    },
    "dependencies": {
        "app-root-path": "^2.0.0",
        "colors": "^1.1.2",
        "gulp-util": "^3.0.6",
        "log-symbols": "^1.0.2",
        "path": "^0.12.7",
        "standard": "^10.0.0",
        "through2": "^2.0.0"
    },
    "description": "gulp plugin for checking JavaScript code with the standard syntax",
    "devDependencies": {
        "mocha": "^3.0.2",
        "should": "^11.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "b36b8148a89bfd0f5373890c1b1c7fc9b1868de1",
        "tarball": "https://registry.npmjs.org/gulp-standard/-/gulp-standard-10.0.0.tgz"
    },
    "gitHead": "bfc95731ebd20dfb40129355f3a020479efe3f83",
    "homepage": "https://github.com/emgeee/gulp-standard",
    "keywords": [
        "standard",
        "gulpplugin"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "emgeee"
        }
    ],
    "name": "gulp-standard",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/emgeee/gulp-standard.git"
    },
    "scripts": {
        "fix-style": "standard --verbose --fix",
        "test": "standard --verbose && mocha"
    },
    "standard": {
        "ignore": [
            "test/fixtures/"
        ]
    },
    "version": "10.0.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
