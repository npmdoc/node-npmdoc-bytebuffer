# npmdoc-bytebuffer

#### api documentation for  [bytebuffer (v5.0.1)](https://github.com/dcodeIO/bytebuffer.js#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-bytebuffer.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-bytebuffer) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-bytebuffer.svg)](https://travis-ci.org/npmdoc/node-npmdoc-bytebuffer)

#### The swiss army knife for binary data in JavaScript.

[![NPM](https://nodei.co/npm/bytebuffer.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/bytebuffer)

- [https://npmdoc.github.io/node-npmdoc-bytebuffer/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-bytebuffer/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-bytebuffer/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-bytebuffer/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-bytebuffer/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-bytebuffer/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Daniel Wirtz"
    },
    "browser": "dist/bytebuffer.js",
    "bugs": {
        "url": "https://github.com/dcodeIO/bytebuffer.js/issues"
    },
    "dependencies": {
        "long": "~3"
    },
    "description": "The swiss army knife for binary data in JavaScript.",
    "devDependencies": {
        "closurecompiler": "~1",
        "lxiv": "~0.2",
        "metascript": "~0",
        "pretty-hrtime": "^1.0.0",
        "testjs": "~1",
        "utfx": "^1.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "582eea4b1a873b6d020a48d58df85f0bba6cfddd",
        "tarball": "https://registry.npmjs.org/bytebuffer/-/bytebuffer-5.0.1.tgz"
    },
    "engines": {
        "node": ">=0.8"
    },
    "gitHead": "f3f310b6786e5d44686d385a2cc60c6720a1069b",
    "homepage": "https://github.com/dcodeIO/bytebuffer.js#readme",
    "keywords": [
        "net",
        "array",
        "buffer",
        "arraybuffer",
        "typed array",
        "bytebuffer",
        "json",
        "websocket",
        "webrtc"
    ],
    "license": "Apache-2.0",
    "main": "dist/bytebuffer-node.js",
    "maintainers": [
        {
            "name": "dcode"
        }
    ],
    "name": "bytebuffer",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/dcodeIO/bytebuffer.js.git"
    },
    "scripts": {
        "build": "node scripts/build.js",
        "compile": "npm run-script compile-default && npm run-script compile-dataview",
        "compile-dataview": "ccjs dist/bytebuffer-dataview.js --create_source_map=dist/bytebuffer-dataview.min.map --externs=externs/minimal-env.js --externs=node_modules/long/externs/long.js > dist/bytebuffer-dataview.min.js",
        "compile-default": "ccjs dist/bytebuffer.js --create_source_map=dist/bytebuffer.min.map --externs=externs/minimal-env.js --externs=node_modules/long/externs/long.js > dist/bytebuffer.min.js",
        "compress": "gzip -c -9 dist/bytebuffer.min.js > dist/bytebuffer.min.js.gz && gzip -c -9 dist/bytebuffer-dataview.min.js > dist/bytebuffer-dataview.min.js.gz",
        "make": "npm run-script build && npm run-script compile && npm run-script compress && npm test",
        "prepublish": "npm test",
        "test": "node node_modules/testjs/bin/testjs tests/suite.js"
    },
    "version": "5.0.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
