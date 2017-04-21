# npmtest-release

#### basic test coverage for  [release (v1.2.1)](https://github.com/zeit/release#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-release.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-release) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-release.svg)](https://travis-ci.org/npmtest/node-npmtest-release)

#### Manage GitHub Releases from the command line

[![NPM](https://nodei.co/npm/release.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/release)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-release/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-release/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-release/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-release/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-release/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-release/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-release/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-release/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-release/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-release/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-release/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-release/build/test-report.html](https://npmtest.github.io/node-npmtest-release/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-release/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-release/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-release/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-release/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-release/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-release/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-release/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-release/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "release",
    "version": "1.2.1",
    "description": "Manage GitHub Releases from the command line",
    "scripts": {
        "precommit": "lint-staged",
        "test": "xo"
    },
    "files": [
        "bin",
        "lib"
    ],
    "repository": "zeit/release",
    "keywords": [
        "github",
        "releases",
        "cli",
        "tags",
        "push"
    ],
    "author": "leo",
    "license": "MIT",
    "bin": {
        "release": "./bin/release.js"
    },
    "xo": {
        "extends": [
            "prettier"
        ]
    },
    "lint-staged": {
        "*.js": [
            "npm test",
            "prettier --single-quote --write",
            "git add"
        ]
    },
    "engines": {
        "node": ">= 6.9.0"
    },
    "bugs": {
        "url": "https://github.com/zeit/release/issues"
    },
    "homepage": "https://github.com/zeit/release#readme",
    "devDependencies": {
        "eslint-config-prettier": "1.6.0",
        "husky": "0.13.3",
        "lint-staged": "3.4.0",
        "prettier": "0.22.0",
        "xo": "0.18.1"
    },
    "dependencies": {
        "args": "2.6.0",
        "async-retry": "0.3.0",
        "bluebird": "3.5.0",
        "capitalize": "1.0.0",
        "chalk": "1.1.3",
        "configstore": "3.0.0",
        "git-commits": "1.3.0",
        "git-repo-name": "0.6.0",
        "git-state": "3.1.1",
        "git-username": "0.5.0",
        "github": "9.2.0",
        "inquirer": "3.0.6",
        "node-version": "1.0.0",
        "open": "0.0.5",
        "ora": "1.2.0",
        "pluralize": "4.0.0",
        "random-string": "0.2.0",
        "request": "2.81.0",
        "request-promise-native": "1.0.3",
        "semver": "5.3.0",
        "tagged-versions": "1.3.0",
        "then-sleep": "1.0.1",
        "trim": "0.0.1",
        "update-notifier": "2.1.0"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
