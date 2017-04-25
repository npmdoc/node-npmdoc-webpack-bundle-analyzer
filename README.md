# npmdoc-webpack-bundle-analyzer

#### basic api documentation for  [webpack-bundle-analyzer (v2.4.0)](https://github.com/th0r/webpack-bundle-analyzer)  [![npm package](https://img.shields.io/npm/v/npmdoc-webpack-bundle-analyzer.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-webpack-bundle-analyzer) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-webpack-bundle-analyzer.svg)](https://travis-ci.org/npmdoc/node-npmdoc-webpack-bundle-analyzer)

#### Webpack plugin and CLI utility that represents bundle content as convenient interactive zoomable treemap

[![NPM](https://nodei.co/npm/webpack-bundle-analyzer.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/webpack-bundle-analyzer)

- [https://npmdoc.github.io/node-npmdoc-webpack-bundle-analyzer/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-webpack-bundle-analyzer/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-webpack-bundle-analyzer/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-webpack-bundle-analyzer/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-webpack-bundle-analyzer/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-webpack-bundle-analyzer/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Yury Grunin"
    },
    "bin": {
        "webpack-bundle-analyzer": "lib/bin/analyzer.js"
    },
    "bugs": {
        "url": "https://github.com/th0r/webpack-bundle-analyzer/issues"
    },
    "changelog": "https://github.com/th0r/webpack-bundle-analyzer/blob/master/CHANGELOG.md",
    "dependencies": {
        "acorn": "^5.0.3",
        "chalk": "^1.1.3",
        "commander": "^2.9.0",
        "ejs": "^2.5.6",
        "express": "^4.15.2",
        "filesize": "^3.5.6",
        "gzip-size": "^3.0.0",
        "lodash": "^4.17.4",
        "mkdirp": "^0.5.1",
        "opener": "^1.4.3"
    },
    "description": "Webpack plugin and CLI utility that represents bundle content as convenient interactive zoomable treemap",
    "devDependencies": {
        "babel-core": "6.24.1",
        "babel-eslint": "7.2.1",
        "babel-loader": "6.4.1",
        "babel-plugin-transform-react-jsx": "6.24.1",
        "babel-plugin-transform-runtime": "6.23.0",
        "babel-polyfill": "6.23.0",
        "babel-preset-es2015": "6.24.1",
        "babel-preset-stage-2": "6.24.1",
        "chai": "3.5.0",
        "chai-subset": "1.5.0",
        "classnames": "2.2.5",
        "css-loader": "0.28.0",
        "del": "2.2.2",
        "eslint": "3.19.0",
        "eslint-plugin-react": "6.10.3",
        "exports-loader": "0.6.4",
        "gulp": "3.9.1",
        "gulp-babel": "6.1.2",
        "gulp-plumber": "1.1.0",
        "gulp-util": "3.0.8",
        "gulp-watch": "4.3.11",
        "mocha": "3.2.0",
        "nightmare": "2.10.0",
        "preact": "8.1.0",
        "sinon": "2.1.0",
        "stream-combiner2": "1.1.1",
        "style-loader": "0.16.1",
        "webpack": "2.3.3"
    },
    "directories": {},
    "dist": {
        "shasum": "e406b016e7452bc864793848c79308782accba8e",
        "tarball": "https://registry.npmjs.org/webpack-bundle-analyzer/-/webpack-bundle-analyzer-2.4.0.tgz"
    },
    "engines": {
        "node": ">= 4"
    },
    "files": [
        "public",
        "lib",
        "src",
        "views"
    ],
    "gitHead": "545c680d0a87920a53acbdf52c8c389dd672d043",
    "homepage": "https://github.com/th0r/webpack-bundle-analyzer",
    "keywords": [
        "webpack",
        "bundle",
        "analyzer",
        "modules",
        "size",
        "interactive",
        "chart",
        "treemap",
        "zoomable",
        "zoom"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "th0r"
        }
    ],
    "name": "webpack-bundle-analyzer",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/th0r/webpack-bundle-analyzer.git"
    },
    "scripts": {
        "build": "gulp build",
        "lint": "eslint --ext js,jsx .",
        "npm-publish": "npm run lint && npm run build && npm test && npm publish",
        "start": "gulp watch",
        "test": "mocha --compilers js:babel-core/register -r babel-polyfill",
        "test-dev": "mocha --watch --compilers js:babel-core/register -r babel-polyfill"
    },
    "version": "2.4.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
