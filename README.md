# npmtest-generator-ng2-webpack

#### basic test coverage for  [generator-ng2-webpack (v0.6.7)](https://github.com/cmelion/generator-ng2-webpack)  [![npm package](https://img.shields.io/npm/v/npmtest-generator-ng2-webpack.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-generator-ng2-webpack) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-generator-ng2-webpack.svg)](https://travis-ci.org/npmtest/node-npmtest-generator-ng2-webpack)

#### An opinionated tool for scaffolding an app using angular2 and webpack

[![NPM](https://nodei.co/npm/generator-ng2-webpack.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/generator-ng2-webpack)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-generator-ng2-webpack/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-generator-ng2-webpack/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-generator-ng2-webpack/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-generator-ng2-webpack/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-generator-ng2-webpack/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-generator-ng2-webpack/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-generator-ng2-webpack/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-generator-ng2-webpack/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-generator-ng2-webpack/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-generator-ng2-webpack/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-generator-ng2-webpack/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-generator-ng2-webpack/build/test-report.html](https://npmtest.github.io/node-npmtest-generator-ng2-webpack/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-generator-ng2-webpack/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-generator-ng2-webpack/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-generator-ng2-webpack/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-generator-ng2-webpack/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-generator-ng2-webpack/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-generator-ng2-webpack/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-generator-ng2-webpack/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-generator-ng2-webpack/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "generator-ng2-webpack",
    "version": "0.6.7",
    "description": "An opinionated tool for scaffolding an app using angular2 and webpack",
    "homepage": "https://github.com/cmelion/generator-ng2-webpack",
    "repository": {
        "type": "git",
        "url": "git://github.com/cmelion/generator-ng2-webpack"
    },
    "engines": {
        "node": ">= 4.2.1 <= 5.6.0"
    },
    "scripts": {
        "eslint": "eslint .",
        "lint": "npm run eslint",
        "mocha": "istanbul cover --root ./generators  --include-all-sources -x **/templates/** --dir ./coverage/mocha --report text --report text-summary --report lcov --print none  _mocha -- test/mocha/**/*.spec.js --reporter spec --timeout 10000",
        "mocha:watch": "mocha test/mocha/**/*.spec.js -R nyan -w --timeout 10000",
        "pretest": "npm run eslint",
        "test": "npm run mocha",
        "release:full": "gulp release:full"
    },
    "author": {
        "name": "Charles Fulnecky",
        "url": "https://github.com/cmelion"
    },
    "files": [
        "generators",
        "libs",
        ".jsbeautifyrc"
    ],
    "main": "generators/app/index.js",
    "preferGlobal": true,
    "keywords": [
        "angular 2",
        "angular",
        "angular2",
        "asyncroute",
        "boilerplate",
        "generator",
        "hot-loading",
        "hot-loader",
        "ng2",
        "react",
        "scaffold",
        "starter",
        "typescript",
        "webpack",
        "yeoman",
        "yeoman-generator"
    ],
    "license": "MIT",
    "dependencies": {
        "chalk": "^1.1.1",
        "gulp-filter": "^3.0.1",
        "gulp-tap": "0.1.3",
        "js-beautify": "beautify-web/js-beautify",
        "lodash": "3.10.1",
        "mkdirp": "^0.5.1",
        "repeating": "^2.0.0",
        "string-length": "^1.0.1",
        "strip-json-comments": "^2.0.1",
        "underscore.string": "^3.2.3",
        "update-notifier": "^0.6.0",
        "yeoman-generator": "^0.22.4",
        "yeoman-option-or-prompt": "^1.0.2",
        "yosay": "^1.1.0"
    },
    "devDependencies": {
        "bluebird": "^3.3.1",
        "chai": "^3.5.0",
        "chalk": "1.1.1",
        "coveralls": "^2.11.6",
        "del": "^2.2.0",
        "eslint": "^2.2.0",
        "eslint-plugin-nodeca": "^1.0.3",
        "event-stream": "^3.3.2",
        "github": "0.2.4",
        "github-username": "2.1.0",
        "gulp": "3.9.1",
        "gulp-bump": "1.0.0",
        "gulp-concat": "2.6.0",
        "gulp-exec": "2.1.2",
        "gulp-git": "^1.7.0",
        "gulp-help": "1.6.1",
        "gulp-if": "2.0.0",
        "gulp-order": "1.1.1",
        "gulp-util": "3.0.7",
        "inquirer": "^0.12.0",
        "istanbul": "^0.4.2",
        "mocha": "^2.4.5",
        "node-jsxml": "^0.7.0",
        "require-dir": "0.3.0",
        "run-sequence": "^1.1.5",
        "yargs": "^4.1.0",
        "yeoman-assert": "^2.1.1",
        "yeoman-test": "^1.1.0"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
