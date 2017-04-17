# api documentation for  [natural (v0.5.1)](https://github.com/NaturalNode/natural)  [![npm package](https://img.shields.io/npm/v/npmdoc-natural.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-natural) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-natural.svg)](https://travis-ci.org/npmdoc/node-npmdoc-natural)
#### General natural language (tokenizing, stemming (English, Russian, Spanish), classification, inflection, phonetics, tfidf, WordNet, jaro-winkler, Levenshtein distance, Dice's Coefficient) facilities for node.

[![NPM](https://nodei.co/npm/natural.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/natural)

- [https://npmdoc.github.io/node-npmdoc-natural/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-natural/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-natural/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-natural/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-natural/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-natural/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Chris Umbel"
    },
    "bugs": {
        "url": "https://github.com/NaturalNode/natural/issues"
    },
    "dependencies": {
        "apparatus": ">= 0.0.9",
        "sylvester": ">= 0.0.12",
        "underscore": ">=1.3.1",
        "webworker-threads": ">=0.6.2"
    },
    "description": "General natural language (tokenizing, stemming (English, Russian, Spanish), classification, inflection, phonetics, tfidf, WordNet, jaro-winkler, Levenshtein distance, Dice's Coefficient) facilities for node.",
    "devDependencies": {
        "jasmine-node": "~1.13.1",
        "sinon": "^1.12.2",
        "uubench": "0.0.x"
    },
    "directories": {},
    "dist": {
        "shasum": "99a5c8b7f1be0b2d7f9a7803f596f8cc846b5aaf",
        "tarball": "https://registry.npmjs.org/natural/-/natural-0.5.1.tgz"
    },
    "engines": {
        "node": ">=0.4.10"
    },
    "gitHead": "ae15dd821d61b616bdc2c4b1af915e1a1b7f02a7",
    "homepage": "https://github.com/NaturalNode/natural",
    "keywords": [
        "natural",
        "language",
        "porter",
        "lancaster",
        "stemmer",
        "bayes",
        "classifier",
        "phonetic",
        "metaphone",
        "inflector",
        "wordnet",
        "tf-idf",
        "logistic",
        "regression",
        "doublemetaphone",
        "double",
        "jaro-winkler",
        "levenshtein",
        "distance",
        "tagger"
    ],
    "license": "MIT",
    "main": "./lib/natural/index.js",
    "maintainers": [
        {
            "name": "chrisumbel"
        },
        {
            "name": "kkoch986"
        }
    ],
    "name": "natural",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/NaturalNode/natural.git"
    },
    "scripts": {
        "test": "NODE_PATH=. node_modules/jasmine-node/bin/jasmine-node spec/"
    },
    "version": "0.5.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
