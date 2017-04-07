# api documentation for  [gulp-standard (v9.0.0)](https://github.com/emgeee/gulp-standard)  [![npm package](https://img.shields.io/npm/v/npmdoc-gulp-standard.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gulp-standard) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-standard.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-standard)
#### gulp plugin for checking JavaScript code with the standard syntax

[![NPM](https://nodei.co/npm/gulp-standard.png?downloads=true)](https://www.npmjs.com/package/gulp-standard)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-standard/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gulp-standard_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-standard/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gulp-standard/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gulp-standard/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matt Green",
        "email": "mgreen9@gmail.com",
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
        "standard": "^9.0.0",
        "through2": "^2.0.0"
    },
    "description": "gulp plugin for checking JavaScript code with the standard syntax",
    "devDependencies": {
        "mocha": "^3.0.2",
        "should": "^11.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "57599db57449aeb7992240315b5631d51c079cc7",
        "tarball": "https://registry.npmjs.org/gulp-standard/-/gulp-standard-9.0.0.tgz"
    },
    "gitHead": "a29efdc837306a4eb4efa1f33f807b3747feb7e3",
    "homepage": "https://github.com/emgeee/gulp-standard",
    "keywords": [
        "standard",
        "gulpplugin"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "emgeee",
            "email": "green090@gmail.com"
        }
    ],
    "name": "gulp-standard",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "9.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gulp-standard](#apidoc.module.gulp-standard)
1.  [function <span class="apidocSignatureSpan">gulp-standard.</span>reporter (reporter, opts)](#apidoc.element.gulp-standard.reporter)



# <a name="apidoc.module.gulp-standard"></a>[module gulp-standard](#apidoc.module.gulp-standard)

#### <a name="apidoc.element.gulp-standard.reporter"></a>[function <span class="apidocSignatureSpan">gulp-standard.</span>reporter (reporter, opts)](#apidoc.element.gulp-standard.reporter)
- description and source-code
```javascript
reporter = function (reporter, opts) {
  // Load default reporter
  if (reporter === 'default') return defaultReporter(opts)

  // Load reporter from function
  if (typeof reporter === 'function') return reporter(opts)

  // load built-in reporters
  if (typeof reporter === 'string') {
    try {
      return require('gulp-standard/reporters/' + reporter)(opts)
    } catch (err) {}
  }

  // load full-path or module reporters
  if (typeof reporter === 'string') {
    try {
      return require(reporter)(opts)
    } catch (err) {}
  }
}
```
- example usage
```shell
...
// include the required packages.
var gulp = require('gulp')
var standard = require('gulp-standard')

gulp.task('standard', function () {
  return gulp.src(['./app.js'])
    .pipe(standard())
    .pipe(standard.reporter('default', {
      breakOnError: true,
      quiet: true
    }))
})
'''

## Reporters
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
