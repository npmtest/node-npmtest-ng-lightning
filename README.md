# npmtest-ng-lightning

#### basic test coverage for  ng-lightning (v1.3.0)  [![npm package](https://img.shields.io/npm/v/npmtest-ng-lightning.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-ng-lightning) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-ng-lightning.svg)](https://travis-ci.org/npmtest/node-npmtest-ng-lightning)

#### Native Angular components and directives for Lightning Design System

[![NPM](https://nodei.co/npm/ng-lightning.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/ng-lightning)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-ng-lightning/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-ng-lightning/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-ng-lightning/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-ng-lightning/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-ng-lightning/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-ng-lightning/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-ng-lightning/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-ng-lightning/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-ng-lightning/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-ng-lightning/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-ng-lightning/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-ng-lightning/build/test-report.html](https://npmtest.github.io/node-npmtest-ng-lightning/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-ng-lightning/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-ng-lightning/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-ng-lightning/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-ng-lightning/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ng-lightning/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ng-lightning/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-ng-lightning/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-ng-lightning/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "ng-lightning",
    "version": "1.3.0",
    "description": "Native Angular components and directives for Lightning Design System",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/ng-lightning/ng-lightning.git"
    },
    "bugs": {
        "url": "https://github.com/ng-lightning/ng-lightning/issues"
    },
    "main": "bundles/ng-lightning.umd.js",
    "module": "ng-lightning.js",
    "typings": "ng-lightning.d.ts",
    "scripts": {
        "test": "gulp test",
        "tdd": "gulp tdd",
        "lint": "gulp lint:ts --failOnError=true",
        "docs": "compodoc ./temp/inline -p ./tsconfig.json -d ./docs/",
        "build": "gulp",
        "start": "npm run build && gulp build:watch",
        "demo": "gulp demo:clean && webpack --config ./demo/webpack.config.js --watch",
        "demo:build": "npm run build && gulp demo:ngc && webpack --config ./demo/webpack.config.js",
        "demo:release": "npm run demo:build && node scripts/gh-pages",
        "prerelease": "npm run build && npm test",
        "release": "node scripts/release"
    },
    "keywords": [
        "angular",
        "angular2",
        "lightning",
        "lightning design system",
        "salesforce"
    ],
    "author": "Tasos Bekos <tbekos@gmail.com>",
    "license": "MIT",
    "peerDependencies": {
        "@angular/common": ">=2.0.0",
        "@angular/core": ">=2.0.0",
        "@angular/forms": ">=2.0.0"
    },
    "dependencies": {
        "tether": "^1.2.0"
    },
    "devDependencies": {
        "@angular/common": "^2.4.9",
        "@angular/compiler": "^2.4.9",
        "@angular/compiler-cli": "^2.4.9",
        "@angular/core": "^2.4.9",
        "@angular/forms": "^2.4.9",
        "@angular/http": "^2.4.9",
        "@angular/platform-browser": "^2.4.9",
        "@angular/platform-browser-dynamic": "^2.4.9",
        "@angular/platform-server": "^2.4.9",
        "@angular/router": "^3.4.9",
        "@salesforce-ux/design-system": "^2.2.1",
        "@types/jasmine": "2.5.41",
        "@types/node": "^6.0.56",
        "@types/tether": "^1.4.0",
        "angular-router-loader": "^0.5.0",
        "angular2-template-loader": "^0.6.2",
        "app-root-path": "^2.0.1",
        "awesome-typescript-loader": "^3.0.8",
        "browser-sync": "^2.18.8",
        "browser-sync-webpack-plugin": "^1.1.4",
        "clean-webpack-plugin": "^0.1.15",
        "conventional-changelog-cli": "^1.2.0",
        "copy-webpack-plugin": "^4.0.1",
        "core-js": "^2.4.1",
        "dateformat": "^2.0.0",
        "del": "^2.2.2",
        "gh-pages": "^0.12.0",
        "glob": "^7.1.1",
        "gulp": "gulpjs/gulp#4.0",
        "gulp-cached": "^1.1.1",
        "gulp-inline-ng2-template": "^4.0.0",
        "gulp-tslint": "^7.1.0",
        "gulp-typescript": "^3.1.5",
        "html-loader": "^0.4.5",
        "html-webpack-plugin": "^2.28.0",
        "inquirer": "^1.2.3",
        "jasmine-core": "^2.5.1",
        "jasmine-spec-reporter": "^3.2.0",
        "json-loader": "^0.5.3",
        "karma": "^1.5.0",
        "karma-chrome-launcher": "^2.0.0",
        "karma-coverage": "^1.1.1",
        "karma-firefox-launcher": "^1.0.0",
        "karma-ie-launcher": "^1.0.0",
        "karma-jasmine": "^1.1.0",
        "karma-safari-launcher": "^1.0.0",
        "karma-sauce-launcher": "^1.1.0",
        "karma-sourcemap-loader": "^0.3.6",
        "lazypipe": "^1.0.1",
        "markdown-loader": "^0.1.7",
        "prismjs": "^1.5.1",
        "pug": "^2.0.0-beta6",
        "pug-loader": "^2.3.0",
        "q": "^1.4.1",
        "raw-loader": "^0.5.1",
        "replace": "^0.3.0",
        "request": "^2.79.0",
        "rxjs": "^5.2.0",
        "semver": "^5.3.0",
        "shelljs": "^0.7.6",
        "simple-git": "^1.66.0",
        "systemjs": "^0.20.9",
        "tether": "^1.3.8",
        "tslint": "^4.5.1",
        "typescript": "2.0.10",
        "webpack": "^2.2.1",
        "yargs": "^6.6.0",
        "zone.js": "^0.7.7"
    },
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
