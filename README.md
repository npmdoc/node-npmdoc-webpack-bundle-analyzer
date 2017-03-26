# api documentation for  [webpack-bundle-analyzer (v2.3.1)](https://github.com/th0r/webpack-bundle-analyzer)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-webpack-bundle-analyzer.svg)](https://travis-ci.org/npmdoc/node-npmdoc-webpack-bundle-analyzer)
#### Webpack plugin and CLI utility that represents bundle content as convenient interactive zoomable treemap

[![NPM](https://nodei.co/npm/webpack-bundle-analyzer.png?downloads=true)](https://www.npmjs.com/package/webpack-bundle-analyzer)

[![apidoc](https://npmdoc.github.io/node-npmdoc-webpack-bundle-analyzer/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-webpack-bundle-analyzer_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-webpack-bundle-analyzer/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-webpack-bundle-analyzer/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Yury Grunin",
        "email": "grunin.ya@ya.ru"
    },
    "bin": {
        "webpack-bundle-analyzer": "lib/bin/analyzer.js"
    },
    "bugs": {
        "url": "https://github.com/th0r/webpack-bundle-analyzer/issues"
    },
    "changelog": "https://github.com/th0r/webpack-bundle-analyzer/blob/master/CHANGELOG.md",
    "dependencies": {
        "acorn": "^4.0.11",
        "chalk": "^1.1.3",
        "commander": "^2.9.0",
        "ejs": "^2.5.5",
        "express": "^4.14.1",
        "filesize": "^3.5.4",
        "gzip-size": "^3.0.0",
        "lodash": "^4.17.4",
        "mkdirp": "^0.5.1",
        "opener": "^1.4.2"
    },
    "description": "Webpack plugin and CLI utility that represents bundle content as convenient interactive zoomable treemap",
    "devDependencies": {
        "babel-core": "6.22.1",
        "babel-eslint": "7.1.1",
        "babel-loader": "6.2.10",
        "babel-plugin-transform-react-jsx": "6.22.0",
        "babel-plugin-transform-runtime": "6.22.0",
        "babel-polyfill": "6.22.0",
        "babel-preset-es2015": "6.22.0",
        "babel-preset-stage-2": "6.22.0",
        "chai": "3.5.0",
        "chai-subset": "1.4.0",
        "classnames": "2.2.5",
        "css-loader": "0.26.1",
        "del": "2.2.2",
        "eslint": "3.15.0",
        "eslint-plugin-react": "6.9.0",
        "exports-loader": "0.6.3",
        "gulp": "3.9.1",
        "gulp-babel": "6.1.2",
        "gulp-plumber": "1.1.0",
        "gulp-util": "3.0.8",
        "gulp-watch": "4.3.11",
        "mocha": "3.2.0",
        "nightmare": "2.9.1",
        "preact": "7.2.0",
        "sinon": "1.17.7",
        "stream-combiner2": "1.1.1",
        "style-loader": "0.13.1",
        "webpack": "2.2.1"
    },
    "directories": {},
    "dist": {
        "shasum": "d97f8aadbcce68fc865c5787741d8549359a25cd",
        "tarball": "https://registry.npmjs.org/webpack-bundle-analyzer/-/webpack-bundle-analyzer-2.3.1.tgz"
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
    "gitHead": "2e3dc36ad4b20241f543a48bd5322b611d19dda8",
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
            "name": "th0r",
            "email": "grunin.ya@ya.ru"
        }
    ],
    "name": "webpack-bundle-analyzer",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "2.3.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module webpack-bundle-analyzer](#apidoc.module.webpack-bundle-analyzer)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>BundleAnalyzerPlugin (opts)](#apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>Logger ()](#apidoc.element.webpack-bundle-analyzer.Logger)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>start (bundleStats, opts)](#apidoc.element.webpack-bundle-analyzer.start)
1.  object <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>BundleAnalyzerPlugin.prototype
1.  object <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>Logger.prototype
1.  object <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>analyzer
1.  object <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>parseUtils
1.  object <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>tree
1.  object <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>viewer

#### [module webpack-bundle-analyzer.BundleAnalyzerPlugin](#apidoc.module.webpack-bundle-analyzer.BundleAnalyzerPlugin)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>BundleAnalyzerPlugin (opts)](#apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.BundleAnalyzerPlugin)

#### [module webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype](#apidoc.module.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.</span>apply (compiler)](#apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.apply)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.</span>generateStaticReport (stats)](#apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.generateStaticReport)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.</span>generateStatsFile (stats)](#apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.generateStatsFile)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.</span>startAnalyzerServer (stats)](#apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.startAnalyzerServer)

#### [module webpack-bundle-analyzer.Logger](#apidoc.module.webpack-bundle-analyzer.Logger)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>Logger ()](#apidoc.element.webpack-bundle-analyzer.Logger.Logger)
1.  object <span class="apidocSignatureSpan">webpack-bundle-analyzer.Logger.</span>levels

#### [module webpack-bundle-analyzer.Logger.prototype](#apidoc.module.webpack-bundle-analyzer.Logger.prototype)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.Logger.prototype.</span>_log (level)](#apidoc.element.webpack-bundle-analyzer.Logger.prototype._log)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.Logger.prototype.</span>error ()](#apidoc.element.webpack-bundle-analyzer.Logger.prototype.error)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.Logger.prototype.</span>info ()](#apidoc.element.webpack-bundle-analyzer.Logger.prototype.info)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.Logger.prototype.</span>setLogLevel (level)](#apidoc.element.webpack-bundle-analyzer.Logger.prototype.setLogLevel)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.Logger.prototype.</span>warn ()](#apidoc.element.webpack-bundle-analyzer.Logger.prototype.warn)

#### [module webpack-bundle-analyzer.analyzer](#apidoc.module.webpack-bundle-analyzer.analyzer)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.analyzer.</span>getViewerData (bundleStats, bundleDir, opts)](#apidoc.element.webpack-bundle-analyzer.analyzer.getViewerData)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.analyzer.</span>readStatsFromFile (filename)](#apidoc.element.webpack-bundle-analyzer.analyzer.readStatsFromFile)

#### [module webpack-bundle-analyzer.parseUtils](#apidoc.module.webpack-bundle-analyzer.parseUtils)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.parseUtils.</span>parseBundle (bundlePath)](#apidoc.element.webpack-bundle-analyzer.parseUtils.parseBundle)

#### [module webpack-bundle-analyzer.tree](#apidoc.module.webpack-bundle-analyzer.tree)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.tree.</span>Folder (name, parent)](#apidoc.element.webpack-bundle-analyzer.tree.Folder)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.tree.</span>Module (name, data, parent)](#apidoc.element.webpack-bundle-analyzer.tree.Module)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.tree.</span>Node (name, parent)](#apidoc.element.webpack-bundle-analyzer.tree.Node)

#### [module webpack-bundle-analyzer.viewer](#apidoc.module.webpack-bundle-analyzer.viewer)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.viewer.</span>generateReport (bundleStats, opts)](#apidoc.element.webpack-bundle-analyzer.viewer.generateReport)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.viewer.</span>start (bundleStats, opts)](#apidoc.element.webpack-bundle-analyzer.viewer.start)
1.  [function <span class="apidocSignatureSpan">webpack-bundle-analyzer.viewer.</span>startServer (bundleStats, opts)](#apidoc.element.webpack-bundle-analyzer.viewer.startServer)



# <a name="apidoc.module.webpack-bundle-analyzer"></a>[module webpack-bundle-analyzer](#apidoc.module.webpack-bundle-analyzer)

#### <a name="apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>BundleAnalyzerPlugin (opts)](#apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin)
- description and source-code
```javascript
function BundleAnalyzerPlugin(opts) {
  _classCallCheck(this, BundleAnalyzerPlugin);

  this.opts = _extends({
    analyzerMode: 'server',
    analyzerHost: '127.0.0.1',
    analyzerPort: 8888,
    reportFilename: 'report.html',
    openAnalyzer: true,
    generateStatsFile: false,
    statsFilename: 'stats.json',
    statsOptions: null,
    logLevel: 'info',
    // deprecated
    startAnalyzer: true
  }, opts);

  this.logger = new Logger(this.opts.logLevel);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-bundle-analyzer.Logger"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>Logger ()](#apidoc.element.webpack-bundle-analyzer.Logger)
- description and source-code
```javascript
function Logger() {
  var level = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : 'info';

  _classCallCheck(this, Logger);

  this.activeLevels = new Set();
  this.setLogLevel(level);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-bundle-analyzer.start"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>start (bundleStats, opts)](#apidoc.element.webpack-bundle-analyzer.start)
- description and source-code
```javascript
function startServer(bundleStats, opts) {
  var _ref = opts || {},
      _ref$port = _ref.port,
      port = _ref$port === undefined ? 8888 : _ref$port,
      _ref$host = _ref.host,
      host = _ref$host === undefined ? '127.0.0.1' : _ref$host,
      _ref$openBrowser = _ref.openBrowser,
      openBrowser = _ref$openBrowser === undefined ? true : _ref$openBrowser,
      _ref$bundleDir = _ref.bundleDir,
      bundleDir = _ref$bundleDir === undefined ? null : _ref$bundleDir,
      _ref$logger = _ref.logger,
      logger = _ref$logger === undefined ? new Logger() : _ref$logger;

  var chartData = getChartData(logger, bundleStats, bundleDir);

  if (!chartData) return;

  var app = express();

  // Explicitly using our 'ejs' dependency to render templates
  // Fixes #17
  app.engine('ejs', require('ejs').renderFile);
  app.set('view engine', 'ejs');
  app.set('views', projectRoot + '/views');
  app.use(express.static(projectRoot + '/public'));

  app.use('/', function (req, res) {
    res.render('viewer', {
      mode: 'server',
      chartData: JSON.stringify(chartData)
    });
  });

  return app.listen(port, host, function () {
    var url = 'http://' + host + ':' + port;

    logger.info(bold('Webpack Bundle Analyzer') + ' is started at ' + bold(url) + '\n' + ('Use ' + bold('Ctrl+C') + ' to close it
'));

    if (openBrowser) {
      opener(url);
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.webpack-bundle-analyzer.BundleAnalyzerPlugin"></a>[module webpack-bundle-analyzer.BundleAnalyzerPlugin](#apidoc.module.webpack-bundle-analyzer.BundleAnalyzerPlugin)

#### <a name="apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.BundleAnalyzerPlugin"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>BundleAnalyzerPlugin (opts)](#apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.BundleAnalyzerPlugin)
- description and source-code
```javascript
function BundleAnalyzerPlugin(opts) {
  _classCallCheck(this, BundleAnalyzerPlugin);

  this.opts = _extends({
    analyzerMode: 'server',
    analyzerHost: '127.0.0.1',
    analyzerPort: 8888,
    reportFilename: 'report.html',
    openAnalyzer: true,
    generateStatsFile: false,
    statsFilename: 'stats.json',
    statsOptions: null,
    logLevel: 'info',
    // deprecated
    startAnalyzer: true
  }, opts);

  this.logger = new Logger(this.opts.logLevel);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype"></a>[module webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype](#apidoc.module.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype)

#### <a name="apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.apply"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.</span>apply (compiler)](#apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.apply)
- description and source-code
```javascript
function apply(compiler) {
  var _this = this;

  this.compiler = compiler;

  compiler.plugin('done', function (stats) {
    stats = stats.toJson(_this.opts.statsOptions);

    var actions = [];

    if (_this.opts.generateStatsFile) {
      actions.push(function () {
        return _this.generateStatsFile(stats);
      });
    }

    // Handling deprecated 'startAnalyzer' flag
    if (_this.opts.analyzerMode === 'server' && !_this.opts.startAnalyzer) {
      _this.opts.analyzerMode = 'disabled';
    }

    if (_this.opts.analyzerMode === 'server') {
      actions.push(function () {
        return _this.startAnalyzerServer(stats);
      });
    } else if (_this.opts.analyzerMode === 'static') {
      actions.push(function () {
        return _this.generateStaticReport(stats);
      });
    }

    if (actions.length) {
      // Making analyzer logs to be after all webpack logs in the console
      setImmediate(function () {
        actions.forEach(function (action) {
          return action();
        });
      });
    }
  });
}
```
- example usage
```shell
...
  Logger.prototype._log = function _log(level) {
    var _console;

    for (var _len = arguments.length, args = Array(_len > 1 ? _len - 1 : 0), _key = 1; _key < _len; _key++) {
      args[_key - 1] = arguments[_key];
    }

    (_console = console)[LEVEL_TO_CONSOLE_METHOD.get(level) || level].apply(_console, args);
  };

  return Logger;
}();

Logger.levels = LEVELS;
;
...
```

#### <a name="apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.generateStaticReport"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.</span>generateStaticReport (stats)](#apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.generateStaticReport)
- description and source-code
```javascript
function generateStaticReport(stats) {
  viewer.generateReport(stats, {
    openBrowser: this.opts.openAnalyzer,
    reportFilename: this.opts.reportFilename,
    bundleDir: this.compiler.outputPath,
    logger: this.logger
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.generateStatsFile"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.</span>generateStatsFile (stats)](#apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.generateStatsFile)
- description and source-code
```javascript
function generateStatsFile(stats) {
  var statsFilepath = this.opts.statsFilename;

  if (!path.isAbsolute(statsFilepath)) {
    statsFilepath = path.resolve(this.compiler.outputPath, statsFilepath);
  }

  mkdir.sync(path.dirname(statsFilepath));

  fs.writeFileSync(statsFilepath, JSON.stringify(stats, null, 2));

  this.logger.info(bold('Webpack Bundle Analyzer') + ' saved stats file to ' + bold(statsFilepath));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.startAnalyzerServer"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.</span>startAnalyzerServer (stats)](#apidoc.element.webpack-bundle-analyzer.BundleAnalyzerPlugin.prototype.startAnalyzerServer)
- description and source-code
```javascript
function startAnalyzerServer(stats) {
  viewer.startServer(stats, {
    openBrowser: this.opts.openAnalyzer,
    host: this.opts.analyzerHost,
    port: this.opts.analyzerPort,
    bundleDir: this.compiler.outputPath,
    logger: this.logger
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.webpack-bundle-analyzer.Logger"></a>[module webpack-bundle-analyzer.Logger](#apidoc.module.webpack-bundle-analyzer.Logger)

#### <a name="apidoc.element.webpack-bundle-analyzer.Logger.Logger"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.</span>Logger ()](#apidoc.element.webpack-bundle-analyzer.Logger.Logger)
- description and source-code
```javascript
function Logger() {
  var level = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : 'info';

  _classCallCheck(this, Logger);

  this.activeLevels = new Set();
  this.setLogLevel(level);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.webpack-bundle-analyzer.Logger.prototype"></a>[module webpack-bundle-analyzer.Logger.prototype](#apidoc.module.webpack-bundle-analyzer.Logger.prototype)

#### <a name="apidoc.element.webpack-bundle-analyzer.Logger.prototype._log"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.Logger.prototype.</span>_log (level)](#apidoc.element.webpack-bundle-analyzer.Logger.prototype._log)
- description and source-code
```javascript
function _log(level) {
  var _console;

  for (var _len = arguments.length, args = Array(_len > 1 ? _len - 1 : 0), _key = 1; _key < _len; _key++) {
    args[_key - 1] = arguments[_key];
  }

  (_console = console)[LEVEL_TO_CONSOLE_METHOD.get(level) || level].apply(_console, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-bundle-analyzer.Logger.prototype.error"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.Logger.prototype.</span>error ()](#apidoc.element.webpack-bundle-analyzer.Logger.prototype.error)
- description and source-code
```javascript
error = function () {
  for (var _len2 = arguments.length, args = Array(_len2), _key2 = 0; _key2 < _len2; _key2++) {
    args[_key2] = arguments[_key2];
  }

  if (this.activeLevels.has(level)) this._log.apply(this, [level].concat(args));
}
```
- example usage
```shell
...
  if (!chartData) return;

  ejs.renderFile(projectRoot + '/views/viewer.ejs', {
mode: 'static',
chartData: JSON.stringify(chartData),
assetContent: getAssetContent
  }, function (err, reportHtml) {
if (err) return logger.error(err);

var reportFilepath = reportFilename;

if (!path.isAbsolute(reportFilepath)) {
  reportFilepath = path.resolve(bundleDir || process.cwd(), reportFilepath);
}
...
```

#### <a name="apidoc.element.webpack-bundle-analyzer.Logger.prototype.info"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.Logger.prototype.</span>info ()](#apidoc.element.webpack-bundle-analyzer.Logger.prototype.info)
- description and source-code
```javascript
info = function () {
  for (var _len2 = arguments.length, args = Array(_len2), _key2 = 0; _key2 < _len2; _key2++) {
    args[_key2] = arguments[_key2];
  }

  if (this.activeLevels.has(level)) this._log.apply(this, [level].concat(args));
}
```
- example usage
```shell
...
      chartData: JSON.stringify(chartData)
    });
  });

  return app.listen(port, host, function () {
    var url = 'http://' + host + ':' + port;

    logger.info(bold('Webpack Bundle Analyzer') + ' is started at ' + bold(url) + '\n' + ('Use ' + bold('Ctrl+C') + ' to close it
'));

    if (openBrowser) {
      opener(url);
    }
  });
}
...
```

#### <a name="apidoc.element.webpack-bundle-analyzer.Logger.prototype.setLogLevel"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.Logger.prototype.</span>setLogLevel (level)](#apidoc.element.webpack-bundle-analyzer.Logger.prototype.setLogLevel)
- description and source-code
```javascript
function setLogLevel(level) {
  var levelIndex = LEVELS.indexOf(level);

  if (levelIndex === -1) throw new Error('Invalid log level "' + level + '". Use one of these: ' + LEVELS.join(', '));

  this.activeLevels.clear();

  for (var _iterator = LEVELS.entries(), _isArray = Array.isArray(_iterator), _i = 0, _iterator = _isArray ? _iterator : _iterator
[Symbol.iterator]();;) {
    var _ref;

    if (_isArray) {
      if (_i >= _iterator.length) break;
      _ref = _iterator[_i++];
    } else {
      _i = _iterator.next();
      if (_i.done) break;
      _ref = _i.value;
    }

    var _ref2 = _ref,
        i = _ref2[0],
        _level = _ref2[1];

    if (i >= levelIndex) this.activeLevels.add(_level);
  }
}
```
- example usage
```shell
...
var Logger = function () {
  function Logger() {
var level = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : 'info';

_classCallCheck(this, Logger);

this.activeLevels = new Set();
this.setLogLevel(level);
  }

  Logger.prototype.setLogLevel = function setLogLevel(level) {
var levelIndex = LEVELS.indexOf(level);

if (levelIndex === -1) throw new Error('Invalid log level "' + level + '". Use one of these: ' + LEVELS.join(', '));
...
```

#### <a name="apidoc.element.webpack-bundle-analyzer.Logger.prototype.warn"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.Logger.prototype.</span>warn ()](#apidoc.element.webpack-bundle-analyzer.Logger.prototype.warn)
- description and source-code
```javascript
warn = function () {
  for (var _len2 = arguments.length, args = Array(_len2), _key2 = 0; _key2 < _len2; _key2++) {
    args[_key2] = arguments[_key2];
  }

  if (this.activeLevels.has(level)) this._log.apply(this, [level].concat(args));
}
```
- example usage
```shell
...
    bundleInfo = null;
  }

  if (bundleInfo) {
    bundlesSources[statAsset.name] = bundleInfo.src;
    _.assign(parsedModules, bundleInfo.modules);
  } else {
    logger.warn('\nCouldn\'t parse bundle asset "' + assetFile + '".\n' + 'Analyzer will use module sizes from stats file.\n');
    parsedModules = null;
    bundlesSources = null;
    break;
  }
}

if (parsedModules) {
...
```



# <a name="apidoc.module.webpack-bundle-analyzer.analyzer"></a>[module webpack-bundle-analyzer.analyzer](#apidoc.module.webpack-bundle-analyzer.analyzer)

#### <a name="apidoc.element.webpack-bundle-analyzer.analyzer.getViewerData"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.analyzer.</span>getViewerData (bundleStats, bundleDir, opts)](#apidoc.element.webpack-bundle-analyzer.analyzer.getViewerData)
- description and source-code
```javascript
function getViewerData(bundleStats, bundleDir, opts) {
  var _ref = opts || {},
      _ref$logger = _ref.logger,
      logger = _ref$logger === undefined ? new Logger() : _ref$logger;

  // Sometimes all the information is located in 'children' array (e.g. problem in #10)


  if (_.isEmpty(bundleStats.assets) && !_.isEmpty(bundleStats.children)) {
    bundleStats = bundleStats.children[0];
  }

  // Picking only '*.js' assets from bundle that has non-empty 'chunks' array
  bundleStats.assets = _.filter(bundleStats.assets, function (asset) {
    // Removing query part from filename (yes, somebody uses it for some reason and Webpack supports it)
    // See #22
    asset.name = asset.name.replace(FILENAME_QUERY_REGEXP, '');

    return _.endsWith(asset.name, '.js') && !_.isEmpty(asset.chunks);
  });

  // Trying to parse bundle assets and get real module sizes if 'bundleDir' is provided
  var parsedModuleSizes = null;
  var bundlesSources = {};
  var parsedModules = {};

  if (bundleDir) {
    for (var _iterator = bundleStats.assets, _isArray = Array.isArray(_iterator), _i = 0, _iterator = _isArray ? _iterator : _iterator
[Symbol.iterator]();;) {
      var _ref2;

      if (_isArray) {
        if (_i >= _iterator.length) break;
        _ref2 = _iterator[_i++];
      } else {
        _i = _iterator.next();
        if (_i.done) break;
        _ref2 = _i.value;
      }

      var statAsset = _ref2;

      var assetFile = path.join(bundleDir, statAsset.name);
      var bundleInfo = void 0;

      try {
        bundleInfo = parseBundle(assetFile);
      } catch (err) {
        bundleInfo = null;
      }

      if (bundleInfo) {
        bundlesSources[statAsset.name] = bundleInfo.src;
        _.assign(parsedModules, bundleInfo.modules);
      } else {
        logger.warn('\nCouldn\'t parse bundle asset "' + assetFile + '".\n' + 'Analyzer will use module sizes from stats file.\n
');
        parsedModules = null;
        bundlesSources = null;
        break;
      }
    }

    if (parsedModules) {
      parsedModuleSizes = _.mapValues(parsedModules, function (moduleSrc) {
        return {
          raw: moduleSrc.length,
          gzip: gzipSize.sync(moduleSrc)
        };
      });
    }
  }

  var assets = _.transform(bundleStats.assets, function (result, statAsset) {
    var asset = result[statAsset.name] = _.pick(statAsset, 'size');

    if (bundlesSources) {
      asset.parsedSize = bundlesSources[statAsset.name].length;
      asset.gzipSize = gzipSize.sync(bundlesSources[statAsset.name]);
    }

    // Picking modules from current bundle script
    asset.modules = _(bundleStats.modules).filter(function (statModule) {
      return assetHasModule(statAsset, statModule);
    }).each(function (statModule) {
      if (parsedModuleSizes) {
        statModule.parsedSize = parsedModuleSizes[statModule.id].raw;
        statModule.gzipSize = parsedModuleSizes[statModule.id].gzip;
      }
    });

    asset.tree = createModulesTree(asset.modules);
  }, {});

  return _.transform(assets, function (result, asset, filename) {
    result.push({
      label: filename,
      // Not using 'asset.size' here provided by Webpack because it can be very confusing when 'UglifyJsPlugin' is used.
      // In this case all module sizes from stats file will represent unminified module sizes, but 'asset.size' will
      // be the size of minified bundle.
      statSize: asset.tree.size,
      parsedSize: asset.parsedSize,
      gzipSize: asset.gzipSize,
      groups: _.invokeMap(asset.tree.children, 'toChartData')
    });
  }, []);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-bundle-analyzer.analyzer.readStatsFromFile"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.analyzer.</span>readStatsFromFile (filename)](#apidoc.element.webpack-bundle-analyzer.analyzer.readStatsFromFile)
- description and source-code
```javascript
function readStatsFromFile(filename) {
  return JSON.parse(fs.readFileSync(filename, 'utf8'));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.webpack-bundle-analyzer.parseUtils"></a>[module webpack-bundle-analyzer.parseUtils](#apidoc.module.webpack-bundle-analyzer.parseUtils)

#### <a name="apidoc.element.webpack-bundle-analyzer.parseUtils.parseBundle"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.parseUtils.</span>parseBundle (bundlePath)](#apidoc.element.webpack-bundle-analyzer.parseUtils.parseBundle)
- description and source-code
```javascript
function parseBundle(bundlePath) {
  var contentBuffer = fs.readFileSync(bundlePath);
  var contentStr = contentBuffer.toString('utf8');
  var ast = acorn.parse(contentStr, { sourceType: 'script' });

  var walkState = {
    locations: null
  };

  walk.recursive(ast, walkState, {
    CallExpression: function CallExpression(node, state, c) {
      if (state.sizes) return;

      var args = node.arguments;

      // Additional bundle without webpack loader.
      // Modules are stored in second argument, after chunk ids:
      // webpackJsonp([<chunks>], <modules>, ...)
      // As function name may be changed with 'output.jsonpFunction' option we can't rely on it's default name.
      if (node.callee.type === 'Identifier' && args.length >= 2 && isArgumentContainsChunkIds(args[0]) && isArgumentContainsModulesList
(args[1])) {
        state.locations = getModulesLocationFromFunctionArgument(args[1]);
        return;
      }

      // Additional bundle without webpack loader, with module IDs optimized.
      // Modules are stored in second arguments Array(n).concat() call
      // webpackJsonp([<chunks>], Array([minimum ID]).concat([<module>, <module>, ...]))
      // As function name may be changed with 'output.jsonpFunction' option we can't rely on it's default name.
      if (node.callee.type === 'Identifier' && (args.length === 2 || args.length === 3) && isArgumentContainsChunkIds(args[0]) &&
isArgumentArrayConcatContainingChunks(args[1])) {
        state.locations = getModulesLocationFromArrayConcat(args[1]);
        return;
      }

      // Main bundle with webpack loader
      // Modules are stored in first argument:
      // (function (...) {...})(<modules>)
      if (node.callee.type === 'FunctionExpression' && !node.callee.id && args.length === 1 && isArgumentContainsModulesList(args
[0])) {
        state.locations = getModulesLocationFromFunctionArgument(args[0]);
        return;
      }

      // Walking into arguments because some of plugins (e.g. 'DedupePlugin') or some Webpack
      // features (e.g. 'umd' library output) can wrap modules list into additional IIFE.
      _.each(args, function (arg) {
        return c(arg, state);
      });
    }
  });

  if (!walkState.locations) {
    return null;
  }

  return {
    src: contentStr,
    modules: _.mapValues(walkState.locations, function (loc) {
      return contentBuffer.toString('utf8', loc.start, loc.end);
    })
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.webpack-bundle-analyzer.tree"></a>[module webpack-bundle-analyzer.tree](#apidoc.module.webpack-bundle-analyzer.tree)

#### <a name="apidoc.element.webpack-bundle-analyzer.tree.Folder"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.tree.</span>Folder (name, parent)](#apidoc.element.webpack-bundle-analyzer.tree.Folder)
- description and source-code
```javascript
function Folder(name, parent) {
  _classCallCheck(this, Folder);

  var _this3 = _possibleConstructorReturn(this, _Node2.call(this, name, parent));

  _this3.children = Object.create(null);
  return _this3;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-bundle-analyzer.tree.Module"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.tree.</span>Module (name, data, parent)](#apidoc.element.webpack-bundle-analyzer.tree.Module)
- description and source-code
```javascript
function Module(name, data, parent) {
  _classCallCheck(this, Module);

  var _this = _possibleConstructorReturn(this, _Node.call(this, name, parent));

  _this.data = data;
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-bundle-analyzer.tree.Node"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.tree.</span>Node (name, parent)](#apidoc.element.webpack-bundle-analyzer.tree.Node)
- description and source-code
```javascript
function Node(name, parent) {
  _classCallCheck(this, Node);

  this.name = name;
  this.parent = parent;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.webpack-bundle-analyzer.viewer"></a>[module webpack-bundle-analyzer.viewer](#apidoc.module.webpack-bundle-analyzer.viewer)

#### <a name="apidoc.element.webpack-bundle-analyzer.viewer.generateReport"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.viewer.</span>generateReport (bundleStats, opts)](#apidoc.element.webpack-bundle-analyzer.viewer.generateReport)
- description and source-code
```javascript
function generateReport(bundleStats, opts) {
  var _ref2 = opts || {},
      _ref2$openBrowser = _ref2.openBrowser,
      openBrowser = _ref2$openBrowser === undefined ? true : _ref2$openBrowser,
      _ref2$reportFilename = _ref2.reportFilename,
      reportFilename = _ref2$reportFilename === undefined ? 'report.html' : _ref2$reportFilename,
      _ref2$bundleDir = _ref2.bundleDir,
      bundleDir = _ref2$bundleDir === undefined ? null : _ref2$bundleDir,
      _ref2$logger = _ref2.logger,
      logger = _ref2$logger === undefined ? new Logger() : _ref2$logger;

  var chartData = getChartData(logger, bundleStats, bundleDir);

  if (!chartData) return;

  ejs.renderFile(projectRoot + '/views/viewer.ejs', {
    mode: 'static',
    chartData: JSON.stringify(chartData),
    assetContent: getAssetContent
  }, function (err, reportHtml) {
    if (err) return logger.error(err);

    var reportFilepath = reportFilename;

    if (!path.isAbsolute(reportFilepath)) {
      reportFilepath = path.resolve(bundleDir || process.cwd(), reportFilepath);
    }

    mkdir.sync(path.dirname(reportFilepath));
    fs.writeFileSync(reportFilepath, reportHtml);

    logger.info(bold('Webpack Bundle Analyzer') + ' saved report to ' + bold(reportFilepath));

    if (openBrowser) {
      opener('file://' + reportFilepath);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-bundle-analyzer.viewer.start"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.viewer.</span>start (bundleStats, opts)](#apidoc.element.webpack-bundle-analyzer.viewer.start)
- description and source-code
```javascript
function startServer(bundleStats, opts) {
  var _ref = opts || {},
      _ref$port = _ref.port,
      port = _ref$port === undefined ? 8888 : _ref$port,
      _ref$host = _ref.host,
      host = _ref$host === undefined ? '127.0.0.1' : _ref$host,
      _ref$openBrowser = _ref.openBrowser,
      openBrowser = _ref$openBrowser === undefined ? true : _ref$openBrowser,
      _ref$bundleDir = _ref.bundleDir,
      bundleDir = _ref$bundleDir === undefined ? null : _ref$bundleDir,
      _ref$logger = _ref.logger,
      logger = _ref$logger === undefined ? new Logger() : _ref$logger;

  var chartData = getChartData(logger, bundleStats, bundleDir);

  if (!chartData) return;

  var app = express();

  // Explicitly using our 'ejs' dependency to render templates
  // Fixes #17
  app.engine('ejs', require('ejs').renderFile);
  app.set('view engine', 'ejs');
  app.set('views', projectRoot + '/views');
  app.use(express.static(projectRoot + '/public'));

  app.use('/', function (req, res) {
    res.render('viewer', {
      mode: 'server',
      chartData: JSON.stringify(chartData)
    });
  });

  return app.listen(port, host, function () {
    var url = 'http://' + host + ':' + port;

    logger.info(bold('Webpack Bundle Analyzer') + ' is started at ' + bold(url) + '\n' + ('Use ' + bold('Ctrl+C') + ' to close it
'));

    if (openBrowser) {
      opener(url);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-bundle-analyzer.viewer.startServer"></a>[function <span class="apidocSignatureSpan">webpack-bundle-analyzer.viewer.</span>startServer (bundleStats, opts)](#apidoc.element.webpack-bundle-analyzer.viewer.startServer)
- description and source-code
```javascript
function startServer(bundleStats, opts) {
  var _ref = opts || {},
      _ref$port = _ref.port,
      port = _ref$port === undefined ? 8888 : _ref$port,
      _ref$host = _ref.host,
      host = _ref$host === undefined ? '127.0.0.1' : _ref$host,
      _ref$openBrowser = _ref.openBrowser,
      openBrowser = _ref$openBrowser === undefined ? true : _ref$openBrowser,
      _ref$bundleDir = _ref.bundleDir,
      bundleDir = _ref$bundleDir === undefined ? null : _ref$bundleDir,
      _ref$logger = _ref.logger,
      logger = _ref$logger === undefined ? new Logger() : _ref$logger;

  var chartData = getChartData(logger, bundleStats, bundleDir);

  if (!chartData) return;

  var app = express();

  // Explicitly using our 'ejs' dependency to render templates
  // Fixes #17
  app.engine('ejs', require('ejs').renderFile);
  app.set('view engine', 'ejs');
  app.set('views', projectRoot + '/views');
  app.use(express.static(projectRoot + '/public'));

  app.use('/', function (req, res) {
    res.render('viewer', {
      mode: 'server',
      chartData: JSON.stringify(chartData)
    });
  });

  return app.listen(port, host, function () {
    var url = 'http://' + host + ':' + port;

    logger.info(bold('Webpack Bundle Analyzer') + ' is started at ' + bold(url) + '\n' + ('Use ' + bold('Ctrl+C') + ' to close it
'));

    if (openBrowser) {
      opener(url);
    }
  });
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
