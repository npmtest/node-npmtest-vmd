# npmtest-vmd

#### basic test coverage for  vmd (v1.29.0)  [![npm package](https://img.shields.io/npm/v/npmtest-vmd.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-vmd) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-vmd.svg)](https://travis-ci.org/npmtest/node-npmtest-vmd)

#### vmd

[![NPM](https://nodei.co/npm/vmd.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/vmd)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-vmd/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-vmd/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-vmd/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-vmd/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-vmd/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-vmd/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-vmd/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-vmd/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-vmd/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-vmd/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-vmd/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-vmd/build/test-report.html](https://npmtest.github.io/node-npmtest-vmd/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-vmd/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-vmd/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-vmd/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-vmd/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-vmd/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-vmd/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-vmd/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-vmd/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "vmd",
    "version": "1.29.0",
    "description": "vmd",
    "main": "main/main.js",
    "scripts": {
        "start": "electron main/main.js --not-packaged=true",
        "dev": "electron main/main.js --not-packaged=true --debug=true",
        "test": "standard",
        "pack-linux-ia32": "electron-packager . --asar --overwrite --platform=linux --arch=ia32 --icon=assets/app-icon/png/64.png --prune=true --out=build",
        "pack-linux-x64": "electron-packager . --asar --overwrite --platform=linux --arch=x64 --icon=assets/app-icon/png/64.png --prune=true --out=build",
        "pack-win32-ia32": "electron-packager . --asar  --overwrite --platform=win32 --arch=ia32 --icon=assets/app-icon/win/app.ico --prune=true --out=build --version-string.ProductName='vmd'",
        "pack-win32-x64": "electron-packager . --asar  --overwrite --platform=win32 --arch=x64 --icon=assets/app-icon/win/app.ico --prune=true --out=build --version-string.ProductName='vmd'",
        "pack-mac": "electron-packager . --asar --overwrite --platform=darwin --arch=x64 --icon=assets/app-icon/mac/app.icns --prune=true --out=build",
        "package": "npm run pack-linux-ia32 && npm run pack-linux-x64 && npm run pack-win32-ia32 && npm run pack-win32-x64 && npm run pack-mac",
        "release": "node ./script/release.js"
    },
    "bin": {
        "vmd": "./bin/cli.js"
    },
    "repository": "yoshuawuyts/vmd",
    "keywords": [
        "md",
        "markdown",
        "viewer",
        "browser",
        "standalone",
        "preview",
        "github"
    ],
    "license": "MIT",
    "dependencies": {
        "chokidar": "1.6.1",
        "deep-equal": "1.0.1",
        "electron": "1.4.15",
        "electron-window-state": "4.0.2",
        "emojify.js": "1.1.0",
        "get-stdin": "5.0.1",
        "github-markdown-css": "2.4.1",
        "lodash.template": "4.4.0",
        "mdast-util-to-string": "^1.0.2",
        "minimist": "1.2.0",
        "object-assign": "4.1.1",
        "postcss": "5.2.14",
        "postcss-safe-important": "1.0.4",
        "redux": "3.6.0",
        "remark": "^6.2.0",
        "remark-emoji-to-gemoji": "^1.0.0",
        "remark-highlight.js": "^4.0.1",
        "remark-html": "^5.2.0",
        "remark-slug": "^4.2.2",
        "rucola": "1.1.3",
        "unist-util-visit": "^1.1.1"
    },
    "devDependencies": {
        "electron-packager": "8.5.1",
        "promise-retryer": "0.0.1",
        "request": "2.79.0",
        "standard": "8.6.0"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
