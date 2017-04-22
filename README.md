# npmdoc-mithril

#### api documentation for  mithril (v1.1.1)  [![npm package](https://img.shields.io/npm/v/npmdoc-mithril.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mithril) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mithril.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mithril)

#### A framework for building brilliant applications

[![NPM](https://nodei.co/npm/mithril.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/mithril)

- [https://npmdoc.github.io/node-npmdoc-mithril/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-mithril/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mithril/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mithril/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mithril/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mithril/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "mithril",
    "version": "1.1.1",
    "description": "A framework for building brilliant applications",
    "author": "Leo Horie",
    "license": "MIT",
    "main": "mithril.js",
    "repository": "lhorie/mithril.js",
    "scripts": {
        "dev": "node bundler/cli browser.js -o mithril.js -w",
        "build": "npm run build-browser & npm run build-min",
        "build-browser": "node bundler/cli browser.js -o mithril.js",
        "build-min": "node bundler/cli browser.js -o mithril.min.js -m",
        "lintdocs": "node docs/lint",
        "gendocs": "node docs/generate",
        "lint": "eslint .",
        "lint:fix": "eslint . --fix",
        "test": "node ospec/bin/ospec",
        "posttest": "npm run lint || true",
        "cover": "istanbul cover --print both ospec/bin/ospec",
        "release": "npm version -m \"v%s\"",
        "preversion": "npm run test",
        "version": "npm run build && git add mithril.js mithril.min.js",
        "postversion": "git push --follow-tags"
    },
    "devDependencies": {
        "eslint": "^3.16.1",
        "istanbul": "^0.4.3",
        "marked": "^0.3.6"
    },
    "bin": {
        "ospec": "./ospec/bin/ospec",
        "bundle": "./bundler/bin/bundle"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
