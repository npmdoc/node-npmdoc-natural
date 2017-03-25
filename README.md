# api documentation for  [natural (v0.5.0)](https://github.com/NaturalNode/natural)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-natural.svg)](https://travis-ci.org/npmdoc/node-npmdoc-natural)
#### General natural language (tokenizing, stemming (English, Russian, Spanish), classification, inflection, phonetics, tfidf, WordNet, jaro-winkler, Levenshtein distance, Dice's Coefficient) facilities for node.

[![NPM](https://nodei.co/npm/natural.png?downloads=true)](https://www.npmjs.com/package/natural)

[![apidoc](https://npmdoc.github.io/node-npmdoc-natural/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-natural_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-natural/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-natural/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Chris Umbel",
        "email": "chris@chrisumbel.com"
    },
    "bugs": {
        "url": "https://github.com/NaturalNode/natural/issues"
    },
    "dependencies": {
        "apparatus": ">= 0.0.9",
        "sylvester": ">= 0.0.12",
        "underscore": ">=1.3.1"
    },
    "description": "General natural language (tokenizing, stemming (English, Russian, Spanish), classification, inflection, phonetics, tfidf, WordNet, jaro-winkler, Levenshtein distance, Dice's Coefficient) facilities for node.",
    "devDependencies": {
        "jasmine-node": "~1.13.1",
        "uubench": "0.0.x"
    },
    "directories": {},
    "dist": {
        "shasum": "55a9bb68eccf5ece5535486004a57de264ae3180",
        "tarball": "https://registry.npmjs.org/natural/-/natural-0.5.0.tgz"
    },
    "engines": {
        "node": ">=0.4.10"
    },
    "gitHead": "378ec2b1511b8103ac483eb1a3a73ae6c335da3a",
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
            "name": "chrisumbel",
            "email": "chris@chrisumbel.com"
        },
        {
            "name": "kkoch986",
            "email": "kkoch986@gmail.com"
        }
    ],
    "name": "natural",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/NaturalNode/natural.git"
    },
    "scripts": {
        "test": "NODE_PATH=. node_modules/jasmine-node/bin/jasmine-node spec/"
    },
    "version": "0.5.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module natural](#apidoc.module.natural)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizer ()](#apidoc.element.natural.AggressiveTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizer.super_ ()](#apidoc.element.natural.AggressiveTokenizer.super_)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerEs ()](#apidoc.element.natural.AggressiveTokenizerEs)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerFa ()](#apidoc.element.natural.AggressiveTokenizerFa)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerFr ()](#apidoc.element.natural.AggressiveTokenizerFr)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerIt ()](#apidoc.element.natural.AggressiveTokenizerIt)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerNl ()](#apidoc.element.natural.AggressiveTokenizerNl)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerNo ()](#apidoc.element.natural.AggressiveTokenizerNo)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerPl ()](#apidoc.element.natural.AggressiveTokenizerPl)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerPt ()](#apidoc.element.natural.AggressiveTokenizerPt)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerRu ()](#apidoc.element.natural.AggressiveTokenizerRu)
1.  [function <span class="apidocSignatureSpan">natural.</span>BayesClassifier (stemmer, smoothing)](#apidoc.element.natural.BayesClassifier)
1.  [function <span class="apidocSignatureSpan">natural.</span>BayesClassifier.super_ (classifier, stemmer)](#apidoc.element.natural.BayesClassifier.super_)
1.  [function <span class="apidocSignatureSpan">natural.</span>BrillPOSTagger (lexicon, ruleSet)](#apidoc.element.natural.BrillPOSTagger)
1.  [function <span class="apidocSignatureSpan">natural.</span>CaseTokenizer ()](#apidoc.element.natural.CaseTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.</span>CountInflector ()](#apidoc.element.natural.CountInflector)
1.  [function <span class="apidocSignatureSpan">natural.</span>DiceCoefficient (str1, str2)](#apidoc.element.natural.DiceCoefficient)
1.  [function <span class="apidocSignatureSpan">natural.</span>EdgeWeightedDigraph ()](#apidoc.element.natural.EdgeWeightedDigraph)
1.  [function <span class="apidocSignatureSpan">natural.</span>JaroWinklerDistance (s1, s2, dj)](#apidoc.element.natural.JaroWinklerDistance)
1.  [function <span class="apidocSignatureSpan">natural.</span>LevenshteinDistance (source, target, options)](#apidoc.element.natural.LevenshteinDistance)
1.  [function <span class="apidocSignatureSpan">natural.</span>Lexicon (filename, defaultCategory)](#apidoc.element.natural.Lexicon)
1.  [function <span class="apidocSignatureSpan">natural.</span>LogisticRegressionClassifier (stemmer)](#apidoc.element.natural.LogisticRegressionClassifier)
1.  [function <span class="apidocSignatureSpan">natural.</span>LongestPathTree (digraph, start)](#apidoc.element.natural.LongestPathTree)
1.  [function <span class="apidocSignatureSpan">natural.</span>NounInflector ()](#apidoc.element.natural.NounInflector)
1.  [function <span class="apidocSignatureSpan">natural.</span>NounInflector.super_ ()](#apidoc.element.natural.NounInflector.super_)
1.  [function <span class="apidocSignatureSpan">natural.</span>NounInflectorFr ()](#apidoc.element.natural.NounInflectorFr)
1.  [function <span class="apidocSignatureSpan">natural.</span>NounInflectorJa ()](#apidoc.element.natural.NounInflectorJa)
1.  [function <span class="apidocSignatureSpan">natural.</span>PresentVerbInflector ()](#apidoc.element.natural.PresentVerbInflector)
1.  [function <span class="apidocSignatureSpan">natural.</span>RegexpTokenizer (options)](#apidoc.element.natural.RegexpTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.</span>RuleSet (filename)](#apidoc.element.natural.RuleSet)
1.  [function <span class="apidocSignatureSpan">natural.</span>SentenceAnalyzer (pos, callback)](#apidoc.element.natural.SentenceAnalyzer)
1.  [function <span class="apidocSignatureSpan">natural.</span>SentenceTokenizer ()](#apidoc.element.natural.SentenceTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.</span>ShortestPathTree (digraph, start)](#apidoc.element.natural.ShortestPathTree)
1.  [function <span class="apidocSignatureSpan">natural.</span>Spellcheck (wordlist)](#apidoc.element.natural.Spellcheck)
1.  [function <span class="apidocSignatureSpan">natural.</span>StemmerFr ()](#apidoc.element.natural.StemmerFr)
1.  [function <span class="apidocSignatureSpan">natural.</span>StemmerJa ()](#apidoc.element.natural.StemmerJa)
1.  [function <span class="apidocSignatureSpan">natural.</span>StemmerPl ()](#apidoc.element.natural.StemmerPl)
1.  [function <span class="apidocSignatureSpan">natural.</span>TfIdf (deserialized)](#apidoc.element.natural.TfIdf)
1.  [function <span class="apidocSignatureSpan">natural.</span>TokenizerJa ()](#apidoc.element.natural.TokenizerJa)
1.  [function <span class="apidocSignatureSpan">natural.</span>TreebankWordTokenizer ()](#apidoc.element.natural.TreebankWordTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.</span>Trie (caseSensitive)](#apidoc.element.natural.Trie)
1.  [function <span class="apidocSignatureSpan">natural.</span>WordNet (dataDir)](#apidoc.element.natural.WordNet)
1.  [function <span class="apidocSignatureSpan">natural.</span>WordPunctTokenizer (options)](#apidoc.element.natural.WordPunctTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.</span>WordTokenizer (options)](#apidoc.element.natural.WordTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.</span>normalize (tokens)](#apidoc.element.natural.normalize)
1.  [function <span class="apidocSignatureSpan">natural.</span>normalize_ja (str)](#apidoc.element.natural.normalize_ja)
1.  [function <span class="apidocSignatureSpan">natural.</span>removeDiacritics (str)](#apidoc.element.natural.removeDiacritics)
1.  [function <span class="apidocSignatureSpan">natural.</span>transliterate_ja (str)](#apidoc.element.natural.transliterate_ja)
1.  object <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizer.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizer.super_.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerEs.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerFa.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerFr.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerIt.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerNl.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerNo.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerPl.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerPt.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerRu.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>BayesClassifier.super_.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>BrillPOSTagger.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>CaseTokenizer.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>DoubleMetaphone
1.  object <span class="apidocSignatureSpan">natural.</span>EdgeWeightedDigraph.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>LancasterStemmer
1.  object <span class="apidocSignatureSpan">natural.</span>Lexicon.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>LogisticRegressionClassifier.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>LongestPathTree.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>Metaphone
1.  object <span class="apidocSignatureSpan">natural.</span>NGrams
1.  object <span class="apidocSignatureSpan">natural.</span>NGramsZH
1.  object <span class="apidocSignatureSpan">natural.</span>NounInflector.super_.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>PorterStemmer
1.  object <span class="apidocSignatureSpan">natural.</span>PorterStemmerEs
1.  object <span class="apidocSignatureSpan">natural.</span>PorterStemmerFa
1.  object <span class="apidocSignatureSpan">natural.</span>PorterStemmerFr
1.  object <span class="apidocSignatureSpan">natural.</span>PorterStemmerIt
1.  object <span class="apidocSignatureSpan">natural.</span>PorterStemmerNo
1.  object <span class="apidocSignatureSpan">natural.</span>PorterStemmerPt
1.  object <span class="apidocSignatureSpan">natural.</span>PorterStemmerRu
1.  object <span class="apidocSignatureSpan">natural.</span>RegexpTokenizer.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>SentenceAnalyzer.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>SentenceTokenizer.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>ShortestPathTree.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>SoundEx
1.  object <span class="apidocSignatureSpan">natural.</span>SoundExDM
1.  object <span class="apidocSignatureSpan">natural.</span>Spellcheck.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>StemmerJa.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>TfIdf.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>TokenizerJa.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>TreebankWordTokenizer.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>Trie.prototype
1.  object <span class="apidocSignatureSpan">natural.</span>stopwords

#### [module natural.AggressiveTokenizer](#apidoc.module.natural.AggressiveTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizer ()](#apidoc.element.natural.AggressiveTokenizer.AggressiveTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizer.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizer.super_)

#### [module natural.AggressiveTokenizer.prototype](#apidoc.module.natural.AggressiveTokenizer.prototype)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizer.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizer.prototype.tokenize)

#### [module natural.AggressiveTokenizer.super_](#apidoc.module.natural.AggressiveTokenizer.super_)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizer.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizer.super_.super_)

#### [module natural.AggressiveTokenizer.super_.prototype](#apidoc.module.natural.AggressiveTokenizer.super_.prototype)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizer.super_.prototype.</span>attach ()](#apidoc.element.natural.AggressiveTokenizer.super_.prototype.attach)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizer.super_.prototype.</span>tokenize ()](#apidoc.element.natural.AggressiveTokenizer.super_.prototype.tokenize)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizer.super_.prototype.</span>trim (array)](#apidoc.element.natural.AggressiveTokenizer.super_.prototype.trim)

#### [module natural.AggressiveTokenizerEs](#apidoc.module.natural.AggressiveTokenizerEs)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerEs ()](#apidoc.element.natural.AggressiveTokenizerEs.AggressiveTokenizerEs)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerEs.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerEs.super_)

#### [module natural.AggressiveTokenizerEs.prototype](#apidoc.module.natural.AggressiveTokenizerEs.prototype)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerEs.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerEs.prototype.tokenize)

#### [module natural.AggressiveTokenizerFa](#apidoc.module.natural.AggressiveTokenizerFa)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerFa ()](#apidoc.element.natural.AggressiveTokenizerFa.AggressiveTokenizerFa)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerFa.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerFa.super_)

#### [module natural.AggressiveTokenizerFa.prototype](#apidoc.module.natural.AggressiveTokenizerFa.prototype)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerFa.prototype.</span>clearEmptyString (array)](#apidoc.element.natural.AggressiveTokenizerFa.prototype.clearEmptyString)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerFa.prototype.</span>clearText (text)](#apidoc.element.natural.AggressiveTokenizerFa.prototype.clearText)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerFa.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerFa.prototype.tokenize)

#### [module natural.AggressiveTokenizerFr](#apidoc.module.natural.AggressiveTokenizerFr)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerFr ()](#apidoc.element.natural.AggressiveTokenizerFr.AggressiveTokenizerFr)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerFr.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerFr.super_)

#### [module natural.AggressiveTokenizerFr.prototype](#apidoc.module.natural.AggressiveTokenizerFr.prototype)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerFr.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerFr.prototype.tokenize)

#### [module natural.AggressiveTokenizerIt](#apidoc.module.natural.AggressiveTokenizerIt)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerIt ()](#apidoc.element.natural.AggressiveTokenizerIt.AggressiveTokenizerIt)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerIt.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerIt.super_)

#### [module natural.AggressiveTokenizerIt.prototype](#apidoc.module.natural.AggressiveTokenizerIt.prototype)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerIt.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerIt.prototype.tokenize)

#### [module natural.AggressiveTokenizerNl](#apidoc.module.natural.AggressiveTokenizerNl)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerNl ()](#apidoc.element.natural.AggressiveTokenizerNl.AggressiveTokenizerNl)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerNl.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerNl.super_)

#### [module natural.AggressiveTokenizerNl.prototype](#apidoc.module.natural.AggressiveTokenizerNl.prototype)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerNl.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerNl.prototype.tokenize)

#### [module natural.AggressiveTokenizerNo](#apidoc.module.natural.AggressiveTokenizerNo)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerNo ()](#apidoc.element.natural.AggressiveTokenizerNo.AggressiveTokenizerNo)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerNo.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerNo.super_)

#### [module natural.AggressiveTokenizerNo.prototype](#apidoc.module.natural.AggressiveTokenizerNo.prototype)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerNo.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerNo.prototype.tokenize)

#### [module natural.AggressiveTokenizerPl](#apidoc.module.natural.AggressiveTokenizerPl)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerPl ()](#apidoc.element.natural.AggressiveTokenizerPl.AggressiveTokenizerPl)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerPl.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerPl.super_)

#### [module natural.AggressiveTokenizerPl.prototype](#apidoc.module.natural.AggressiveTokenizerPl.prototype)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerPl.prototype.</span>clearText (text)](#apidoc.element.natural.AggressiveTokenizerPl.prototype.clearText)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerPl.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerPl.prototype.tokenize)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerPl.prototype.</span>withoutEmpty (array)](#apidoc.element.natural.AggressiveTokenizerPl.prototype.withoutEmpty)

#### [module natural.AggressiveTokenizerPt](#apidoc.module.natural.AggressiveTokenizerPt)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerPt ()](#apidoc.element.natural.AggressiveTokenizerPt.AggressiveTokenizerPt)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerPt.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerPt.super_)

#### [module natural.AggressiveTokenizerPt.prototype](#apidoc.module.natural.AggressiveTokenizerPt.prototype)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerPt.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerPt.prototype.tokenize)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerPt.prototype.</span>withoutEmpty (array)](#apidoc.element.natural.AggressiveTokenizerPt.prototype.withoutEmpty)

#### [module natural.AggressiveTokenizerRu](#apidoc.module.natural.AggressiveTokenizerRu)
1.  [function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerRu ()](#apidoc.element.natural.AggressiveTokenizerRu.AggressiveTokenizerRu)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerRu.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerRu.super_)

#### [module natural.AggressiveTokenizerRu.prototype](#apidoc.module.natural.AggressiveTokenizerRu.prototype)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerRu.prototype.</span>clearText (text)](#apidoc.element.natural.AggressiveTokenizerRu.prototype.clearText)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerRu.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerRu.prototype.tokenize)
1.  [function <span class="apidocSignatureSpan">natural.AggressiveTokenizerRu.prototype.</span>withoutEmpty (array)](#apidoc.element.natural.AggressiveTokenizerRu.prototype.withoutEmpty)

#### [module natural.BayesClassifier](#apidoc.module.natural.BayesClassifier)
1.  [function <span class="apidocSignatureSpan">natural.</span>BayesClassifier (stemmer, smoothing)](#apidoc.element.natural.BayesClassifier.BayesClassifier)
1.  [function <span class="apidocSignatureSpan">natural.BayesClassifier.</span>load (filename, stemmer, callback)](#apidoc.element.natural.BayesClassifier.load)
1.  [function <span class="apidocSignatureSpan">natural.BayesClassifier.</span>restore (classifier, stemmer)](#apidoc.element.natural.BayesClassifier.restore)
1.  [function <span class="apidocSignatureSpan">natural.BayesClassifier.</span>super_ (classifier, stemmer)](#apidoc.element.natural.BayesClassifier.super_)

#### [module natural.BayesClassifier.super_](#apidoc.module.natural.BayesClassifier.super_)
1.  [function <span class="apidocSignatureSpan">natural.BayesClassifier.</span>super_ (classifier, stemmer)](#apidoc.element.natural.BayesClassifier.super_.super_)
1.  [function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.</span>load (filename, callback)](#apidoc.element.natural.BayesClassifier.super_.load)
1.  [function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.</span>restore (classifier, stemmer)](#apidoc.element.natural.BayesClassifier.super_.restore)

#### [module natural.BayesClassifier.super_.prototype](#apidoc.module.natural.BayesClassifier.super_.prototype)
1.  [function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>addDocument (text, classification)](#apidoc.element.natural.BayesClassifier.super_.prototype.addDocument)
1.  [function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>classify (observation)](#apidoc.element.natural.BayesClassifier.super_.prototype.classify)
1.  [function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>getClassifications (observation)](#apidoc.element.natural.BayesClassifier.super_.prototype.getClassifications)
1.  [function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>removeDocument (text, classification)](#apidoc.element.natural.BayesClassifier.super_.prototype.removeDocument)
1.  [function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>retrain ()](#apidoc.element.natural.BayesClassifier.super_.prototype.retrain)
1.  [function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>save (filename, callback)](#apidoc.element.natural.BayesClassifier.super_.prototype.save)
1.  [function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>textToFeatures (observation)](#apidoc.element.natural.BayesClassifier.super_.prototype.textToFeatures)
1.  [function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>train ()](#apidoc.element.natural.BayesClassifier.super_.prototype.train)

#### [module natural.BrillPOSTagger](#apidoc.module.natural.BrillPOSTagger)
1.  [function <span class="apidocSignatureSpan">natural.</span>BrillPOSTagger (lexicon, ruleSet)](#apidoc.element.natural.BrillPOSTagger.BrillPOSTagger)

#### [module natural.BrillPOSTagger.prototype](#apidoc.module.natural.BrillPOSTagger.prototype)
1.  [function <span class="apidocSignatureSpan">natural.BrillPOSTagger.prototype.</span>tag (sentence)](#apidoc.element.natural.BrillPOSTagger.prototype.tag)

#### [module natural.CaseTokenizer](#apidoc.module.natural.CaseTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.</span>CaseTokenizer ()](#apidoc.element.natural.CaseTokenizer.CaseTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.CaseTokenizer.</span>super_ ()](#apidoc.element.natural.CaseTokenizer.super_)

#### [module natural.CaseTokenizer.prototype](#apidoc.module.natural.CaseTokenizer.prototype)
1.  [function <span class="apidocSignatureSpan">natural.CaseTokenizer.prototype.</span>attach ()](#apidoc.element.natural.CaseTokenizer.prototype.attach)
1.  [function <span class="apidocSignatureSpan">natural.CaseTokenizer.prototype.</span>tokenize (text, preserveApostrophe)](#apidoc.element.natural.CaseTokenizer.prototype.tokenize)

#### [module natural.CountInflector](#apidoc.module.natural.CountInflector)
1.  [function <span class="apidocSignatureSpan">natural.</span>CountInflector ()](#apidoc.element.natural.CountInflector.CountInflector)
1.  [function <span class="apidocSignatureSpan">natural.CountInflector.</span>nth (i)](#apidoc.element.natural.CountInflector.nth)

#### [module natural.DoubleMetaphone](#apidoc.module.natural.DoubleMetaphone)
1.  [function <span class="apidocSignatureSpan">natural.DoubleMetaphone.</span>attach ()](#apidoc.element.natural.DoubleMetaphone.attach)
1.  [function <span class="apidocSignatureSpan">natural.DoubleMetaphone.</span>compare (stringA, stringB)](#apidoc.element.natural.DoubleMetaphone.compare)
1.  [function <span class="apidocSignatureSpan">natural.DoubleMetaphone.</span>isVowel (c)](#apidoc.element.natural.DoubleMetaphone.isVowel)
1.  [function <span class="apidocSignatureSpan">natural.DoubleMetaphone.</span>process (token, maxLength)](#apidoc.element.natural.DoubleMetaphone.process)

#### [module natural.EdgeWeightedDigraph](#apidoc.module.natural.EdgeWeightedDigraph)
1.  [function <span class="apidocSignatureSpan">natural.</span>EdgeWeightedDigraph ()](#apidoc.element.natural.EdgeWeightedDigraph.EdgeWeightedDigraph)

#### [module natural.EdgeWeightedDigraph.prototype](#apidoc.module.natural.EdgeWeightedDigraph.prototype)
1.  [function <span class="apidocSignatureSpan">natural.EdgeWeightedDigraph.prototype.</span>add (start, end, weight)](#apidoc.element.natural.EdgeWeightedDigraph.prototype.add)
1.  [function <span class="apidocSignatureSpan">natural.EdgeWeightedDigraph.prototype.</span>addEdge (e)](#apidoc.element.natural.EdgeWeightedDigraph.prototype.addEdge)
1.  [function <span class="apidocSignatureSpan">natural.EdgeWeightedDigraph.prototype.</span>e ()](#apidoc.element.natural.EdgeWeightedDigraph.prototype.e)
1.  [function <span class="apidocSignatureSpan">natural.EdgeWeightedDigraph.prototype.</span>edges ()](#apidoc.element.natural.EdgeWeightedDigraph.prototype.edges)
1.  [function <span class="apidocSignatureSpan">natural.EdgeWeightedDigraph.prototype.</span>getAdj (v)](#apidoc.element.natural.EdgeWeightedDigraph.prototype.getAdj)
1.  [function <span class="apidocSignatureSpan">natural.EdgeWeightedDigraph.prototype.</span>toString ()](#apidoc.element.natural.EdgeWeightedDigraph.prototype.toString)
1.  [function <span class="apidocSignatureSpan">natural.EdgeWeightedDigraph.prototype.</span>v ()](#apidoc.element.natural.EdgeWeightedDigraph.prototype.v)

#### [module natural.LancasterStemmer](#apidoc.module.natural.LancasterStemmer)
1.  [function <span class="apidocSignatureSpan">natural.LancasterStemmer.</span>addStopWord (stopWord)](#apidoc.element.natural.LancasterStemmer.addStopWord)
1.  [function <span class="apidocSignatureSpan">natural.LancasterStemmer.</span>addStopWords (moreStopWords)](#apidoc.element.natural.LancasterStemmer.addStopWords)
1.  [function <span class="apidocSignatureSpan">natural.LancasterStemmer.</span>attach ()](#apidoc.element.natural.LancasterStemmer.attach)
1.  [function <span class="apidocSignatureSpan">natural.LancasterStemmer.</span>removeStopWord (stopWord)](#apidoc.element.natural.LancasterStemmer.removeStopWord)
1.  [function <span class="apidocSignatureSpan">natural.LancasterStemmer.</span>removeStopWords (moreStopWords)](#apidoc.element.natural.LancasterStemmer.removeStopWords)
1.  [function <span class="apidocSignatureSpan">natural.LancasterStemmer.</span>stem (token)](#apidoc.element.natural.LancasterStemmer.stem)
1.  [function <span class="apidocSignatureSpan">natural.LancasterStemmer.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.LancasterStemmer.tokenizeAndStem)

#### [module natural.Lexicon](#apidoc.module.natural.Lexicon)
1.  [function <span class="apidocSignatureSpan">natural.</span>Lexicon (filename, defaultCategory)](#apidoc.element.natural.Lexicon.Lexicon)

#### [module natural.Lexicon.prototype](#apidoc.module.natural.Lexicon.prototype)
1.  [function <span class="apidocSignatureSpan">natural.Lexicon.prototype.</span>parseLexicon (data)](#apidoc.element.natural.Lexicon.prototype.parseLexicon)
1.  [function <span class="apidocSignatureSpan">natural.Lexicon.prototype.</span>tagWord (word)](#apidoc.element.natural.Lexicon.prototype.tagWord)

#### [module natural.LogisticRegressionClassifier](#apidoc.module.natural.LogisticRegressionClassifier)
1.  [function <span class="apidocSignatureSpan">natural.</span>LogisticRegressionClassifier (stemmer)](#apidoc.element.natural.LogisticRegressionClassifier.LogisticRegressionClassifier)
1.  [function <span class="apidocSignatureSpan">natural.LogisticRegressionClassifier.</span>load (filename, stemmer, callback)](#apidoc.element.natural.LogisticRegressionClassifier.load)
1.  [function <span class="apidocSignatureSpan">natural.LogisticRegressionClassifier.</span>restore (classifier, stemmer)](#apidoc.element.natural.LogisticRegressionClassifier.restore)
1.  [function <span class="apidocSignatureSpan">natural.LogisticRegressionClassifier.</span>super_ (classifier, stemmer)](#apidoc.element.natural.LogisticRegressionClassifier.super_)

#### [module natural.LogisticRegressionClassifier.prototype](#apidoc.module.natural.LogisticRegressionClassifier.prototype)
1.  [function <span class="apidocSignatureSpan">natural.LogisticRegressionClassifier.prototype.</span>train ()](#apidoc.element.natural.LogisticRegressionClassifier.prototype.train)

#### [module natural.LongestPathTree](#apidoc.module.natural.LongestPathTree)
1.  [function <span class="apidocSignatureSpan">natural.</span>LongestPathTree (digraph, start)](#apidoc.element.natural.LongestPathTree.LongestPathTree)

#### [module natural.LongestPathTree.prototype](#apidoc.module.natural.LongestPathTree.prototype)
1.  [function <span class="apidocSignatureSpan">natural.LongestPathTree.prototype.</span>getDistTo (v)](#apidoc.element.natural.LongestPathTree.prototype.getDistTo)
1.  [function <span class="apidocSignatureSpan">natural.LongestPathTree.prototype.</span>hasPathTo (v)](#apidoc.element.natural.LongestPathTree.prototype.hasPathTo)
1.  [function <span class="apidocSignatureSpan">natural.LongestPathTree.prototype.</span>pathTo (v)](#apidoc.element.natural.LongestPathTree.prototype.pathTo)
1.  [function <span class="apidocSignatureSpan">natural.LongestPathTree.prototype.</span>relaxEdge (e)](#apidoc.element.natural.LongestPathTree.prototype.relaxEdge)
1.  [function <span class="apidocSignatureSpan">natural.LongestPathTree.prototype.</span>relaxVertex (digraph, vertex, tree)](#apidoc.element.natural.LongestPathTree.prototype.relaxVertex)

#### [module natural.Metaphone](#apidoc.module.natural.Metaphone)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>attach ()](#apidoc.element.natural.Metaphone.attach)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>cTransform (token)](#apidoc.element.natural.Metaphone.cTransform)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>compare (stringA, stringB)](#apidoc.element.natural.Metaphone.compare)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>dTransform (token)](#apidoc.element.natural.Metaphone.dTransform)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>dedup (token)](#apidoc.element.natural.Metaphone.dedup)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropBafterMAtEnd (token)](#apidoc.element.natural.Metaphone.dropBafterMAtEnd)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropG (token)](#apidoc.element.natural.Metaphone.dropG)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropH (token)](#apidoc.element.natural.Metaphone.dropH)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropInitialLetters (token)](#apidoc.element.natural.Metaphone.dropInitialLetters)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropT (token)](#apidoc.element.natural.Metaphone.dropT)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropVowels (token)](#apidoc.element.natural.Metaphone.dropVowels)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropW (token)](#apidoc.element.natural.Metaphone.dropW)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropY (token)](#apidoc.element.natural.Metaphone.dropY)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>process (token, maxLength)](#apidoc.element.natural.Metaphone.process)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformCK (token)](#apidoc.element.natural.Metaphone.transformCK)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformG (token)](#apidoc.element.natural.Metaphone.transformG)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformPH (token)](#apidoc.element.natural.Metaphone.transformPH)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformQ (token)](#apidoc.element.natural.Metaphone.transformQ)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformS (token)](#apidoc.element.natural.Metaphone.transformS)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformT (token)](#apidoc.element.natural.Metaphone.transformT)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformV (token)](#apidoc.element.natural.Metaphone.transformV)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformWH (token)](#apidoc.element.natural.Metaphone.transformWH)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformX (token)](#apidoc.element.natural.Metaphone.transformX)
1.  [function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformZ (token)](#apidoc.element.natural.Metaphone.transformZ)

#### [module natural.NGrams](#apidoc.module.natural.NGrams)
1.  [function <span class="apidocSignatureSpan">natural.NGrams.</span>bigrams (sequence, startSymbol, endSymbol)](#apidoc.element.natural.NGrams.bigrams)
1.  [function <span class="apidocSignatureSpan">natural.NGrams.</span>multrigrams (sequence, n, startSymbol, endSymbol)](#apidoc.element.natural.NGrams.multrigrams)
1.  [function <span class="apidocSignatureSpan">natural.NGrams.</span>ngrams (sequence, n, startSymbol, endSymbol)](#apidoc.element.natural.NGrams.ngrams)
1.  [function <span class="apidocSignatureSpan">natural.NGrams.</span>setTokenizer (t)](#apidoc.element.natural.NGrams.setTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.NGrams.</span>trigrams (sequence, startSymbol, endSymbol)](#apidoc.element.natural.NGrams.trigrams)

#### [module natural.NGramsZH](#apidoc.module.natural.NGramsZH)
1.  [function <span class="apidocSignatureSpan">natural.NGramsZH.</span>bigrams (sequence, startSymbol, endSymbol)](#apidoc.element.natural.NGramsZH.bigrams)
1.  [function <span class="apidocSignatureSpan">natural.NGramsZH.</span>ngrams (sequence, n, startSymbol, endSymbol)](#apidoc.element.natural.NGramsZH.ngrams)
1.  [function <span class="apidocSignatureSpan">natural.NGramsZH.</span>trigrams (sequence, startSymbol, endSymbol)](#apidoc.element.natural.NGramsZH.trigrams)

#### [module natural.NounInflector](#apidoc.module.natural.NounInflector)
1.  [function <span class="apidocSignatureSpan">natural.</span>NounInflector ()](#apidoc.element.natural.NounInflector.NounInflector)
1.  [function <span class="apidocSignatureSpan">natural.NounInflector.</span>super_ ()](#apidoc.element.natural.NounInflector.super_)

#### [module natural.NounInflector.super_](#apidoc.module.natural.NounInflector.super_)
1.  [function <span class="apidocSignatureSpan">natural.NounInflector.</span>super_ ()](#apidoc.element.natural.NounInflector.super_.super_)

#### [module natural.NounInflector.super_.prototype](#apidoc.module.natural.NounInflector.super_.prototype)
1.  [function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>addForm (singularTable, pluralTable, singular, plural)](#apidoc.element.natural.NounInflector.super_.prototype.addForm)
1.  [function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>addIrregular (singular, plural)](#apidoc.element.natural.NounInflector.super_.prototype.addIrregular)
1.  [function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>addPlural (pattern, replacement)](#apidoc.element.natural.NounInflector.super_.prototype.addPlural)
1.  [function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>addSingular (pattern, replacement)](#apidoc.element.natural.NounInflector.super_.prototype.addSingular)
1.  [function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>ize (token, formSet, customForms)](#apidoc.element.natural.NounInflector.super_.prototype.ize)
1.  [function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>izeAbiguous (token)](#apidoc.element.natural.NounInflector.super_.prototype.izeAbiguous)
1.  [function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>izeRegExps (token, forms)](#apidoc.element.natural.NounInflector.super_.prototype.izeRegExps)
1.  [function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>izeRegulars (token, formSet)](#apidoc.element.natural.NounInflector.super_.prototype.izeRegulars)
1.  [function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>pluralize (token)](#apidoc.element.natural.NounInflector.super_.prototype.pluralize)
1.  [function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>restoreCase (token)](#apidoc.element.natural.NounInflector.super_.prototype.restoreCase)
1.  [function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>singularize (token)](#apidoc.element.natural.NounInflector.super_.prototype.singularize)

#### [module natural.NounInflectorFr](#apidoc.module.natural.NounInflectorFr)
1.  [function <span class="apidocSignatureSpan">natural.</span>NounInflectorFr ()](#apidoc.element.natural.NounInflectorFr.NounInflectorFr)
1.  [function <span class="apidocSignatureSpan">natural.NounInflectorFr.</span>super_ ()](#apidoc.element.natural.NounInflectorFr.super_)

#### [module natural.NounInflectorJa](#apidoc.module.natural.NounInflectorJa)
1.  [function <span class="apidocSignatureSpan">natural.</span>NounInflectorJa ()](#apidoc.element.natural.NounInflectorJa.NounInflectorJa)
1.  [function <span class="apidocSignatureSpan">natural.NounInflectorJa.</span>super_ ()](#apidoc.element.natural.NounInflectorJa.super_)

#### [module natural.PorterStemmer](#apidoc.module.natural.PorterStemmer)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>addStopWord (stopWord)](#apidoc.element.natural.PorterStemmer.addStopWord)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>addStopWords (moreStopWords)](#apidoc.element.natural.PorterStemmer.addStopWords)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>attach ()](#apidoc.element.natural.PorterStemmer.attach)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>categorizeGroups (token)](#apidoc.element.natural.PorterStemmer.categorizeGroups)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>measure (token)](#apidoc.element.natural.PorterStemmer.measure)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>removeStopWord (stopWord)](#apidoc.element.natural.PorterStemmer.removeStopWord)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>removeStopWords (moreStopWords)](#apidoc.element.natural.PorterStemmer.removeStopWords)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>stem (token)](#apidoc.element.natural.PorterStemmer.stem)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step1a (token)](#apidoc.element.natural.PorterStemmer.step1a)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step1b (token)](#apidoc.element.natural.PorterStemmer.step1b)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step1c (token)](#apidoc.element.natural.PorterStemmer.step1c)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step2 (token)](#apidoc.element.natural.PorterStemmer.step2)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step3 (token)](#apidoc.element.natural.PorterStemmer.step3)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step4 (token)](#apidoc.element.natural.PorterStemmer.step4)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step5a (token)](#apidoc.element.natural.PorterStemmer.step5a)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step5b (token)](#apidoc.element.natural.PorterStemmer.step5b)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmer.tokenizeAndStem)

#### [module natural.PorterStemmerEs](#apidoc.module.natural.PorterStemmerEs)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerEs.</span>attach ()](#apidoc.element.natural.PorterStemmerEs.attach)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerEs.</span>stem (token)](#apidoc.element.natural.PorterStemmerEs.stem)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerEs.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmerEs.tokenizeAndStem)

#### [module natural.PorterStemmerFa](#apidoc.module.natural.PorterStemmerFa)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerFa.</span>attach ()](#apidoc.element.natural.PorterStemmerFa.attach)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerFa.</span>stem (token)](#apidoc.element.natural.PorterStemmerFa.stem)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerFa.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmerFa.tokenizeAndStem)

#### [module natural.PorterStemmerFr](#apidoc.module.natural.PorterStemmerFr)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerFr.</span>attach ()](#apidoc.element.natural.PorterStemmerFr.attach)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerFr.</span>endsinArr (token, suffixes)](#apidoc.element.natural.PorterStemmerFr.endsinArr)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerFr.</span>prelude (token)](#apidoc.element.natural.PorterStemmerFr.prelude)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerFr.</span>regions (token)](#apidoc.element.natural.PorterStemmerFr.regions)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerFr.</span>stem (token)](#apidoc.element.natural.PorterStemmerFr.stem)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerFr.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmerFr.tokenizeAndStem)

#### [module natural.PorterStemmerIt](#apidoc.module.natural.PorterStemmerIt)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerIt.</span>attach ()](#apidoc.element.natural.PorterStemmerIt.attach)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerIt.</span>stem (token)](#apidoc.element.natural.PorterStemmerIt.stem)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerIt.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmerIt.tokenizeAndStem)

#### [module natural.PorterStemmerNo](#apidoc.module.natural.PorterStemmerNo)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>addStopWord (stopWord)](#apidoc.element.natural.PorterStemmerNo.addStopWord)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>addStopWords (moreStopWords)](#apidoc.element.natural.PorterStemmerNo.addStopWords)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>attach ()](#apidoc.element.natural.PorterStemmerNo.attach)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>getR1 (token)](#apidoc.element.natural.PorterStemmerNo.getR1)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>stem (token)](#apidoc.element.natural.PorterStemmerNo.stem)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>step1 (token)](#apidoc.element.natural.PorterStemmerNo.step1)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>step1a (token)](#apidoc.element.natural.PorterStemmerNo.step1a)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>step1b (token)](#apidoc.element.natural.PorterStemmerNo.step1b)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>step1c (token)](#apidoc.element.natural.PorterStemmerNo.step1c)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>step2 (token)](#apidoc.element.natural.PorterStemmerNo.step2)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>step3 (token)](#apidoc.element.natural.PorterStemmerNo.step3)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmerNo.tokenizeAndStem)

#### [module natural.PorterStemmerPt](#apidoc.module.natural.PorterStemmerPt)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerPt.</span>addStopWords (words)](#apidoc.element.natural.PorterStemmerPt.addStopWords)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerPt.</span>attach ()](#apidoc.element.natural.PorterStemmerPt.attach)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerPt.</span>stem (word)](#apidoc.element.natural.PorterStemmerPt.stem)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerPt.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmerPt.tokenizeAndStem)

#### [module natural.PorterStemmerRu](#apidoc.module.natural.PorterStemmerRu)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerRu.</span>attach ()](#apidoc.element.natural.PorterStemmerRu.attach)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerRu.</span>stem (token)](#apidoc.element.natural.PorterStemmerRu.stem)
1.  [function <span class="apidocSignatureSpan">natural.PorterStemmerRu.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmerRu.tokenizeAndStem)

#### [module natural.PresentVerbInflector](#apidoc.module.natural.PresentVerbInflector)
1.  [function <span class="apidocSignatureSpan">natural.</span>PresentVerbInflector ()](#apidoc.element.natural.PresentVerbInflector.PresentVerbInflector)
1.  [function <span class="apidocSignatureSpan">natural.PresentVerbInflector.</span>super_ ()](#apidoc.element.natural.PresentVerbInflector.super_)

#### [module natural.RegexpTokenizer](#apidoc.module.natural.RegexpTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.</span>RegexpTokenizer (options)](#apidoc.element.natural.RegexpTokenizer.RegexpTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.RegexpTokenizer.</span>super_ ()](#apidoc.element.natural.RegexpTokenizer.super_)

#### [module natural.RegexpTokenizer.prototype](#apidoc.module.natural.RegexpTokenizer.prototype)
1.  [function <span class="apidocSignatureSpan">natural.RegexpTokenizer.prototype.</span>tokenize (s)](#apidoc.element.natural.RegexpTokenizer.prototype.tokenize)

#### [module natural.SentenceAnalyzer](#apidoc.module.natural.SentenceAnalyzer)
1.  [function <span class="apidocSignatureSpan">natural.</span>SentenceAnalyzer (pos, callback)](#apidoc.element.natural.SentenceAnalyzer.SentenceAnalyzer)

#### [module natural.SentenceAnalyzer.prototype](#apidoc.module.natural.SentenceAnalyzer.prototype)
1.  [function <span class="apidocSignatureSpan">natural.SentenceAnalyzer.prototype.</span>implicitYou ()](#apidoc.element.natural.SentenceAnalyzer.prototype.implicitYou)
1.  [function <span class="apidocSignatureSpan">natural.SentenceAnalyzer.prototype.</span>part (callback)](#apidoc.element.natural.SentenceAnalyzer.prototype.part)
1.  [function <span class="apidocSignatureSpan">natural.SentenceAnalyzer.prototype.</span>predicateToString ()](#apidoc.element.natural.SentenceAnalyzer.prototype.predicateToString)
1.  [function <span class="apidocSignatureSpan">natural.SentenceAnalyzer.prototype.</span>prepositionPhrases ()](#apidoc.element.natural.SentenceAnalyzer.prototype.prepositionPhrases)
1.  [function <span class="apidocSignatureSpan">natural.SentenceAnalyzer.prototype.</span>subjectToString ()](#apidoc.element.natural.SentenceAnalyzer.prototype.subjectToString)
1.  [function <span class="apidocSignatureSpan">natural.SentenceAnalyzer.prototype.</span>toString ()](#apidoc.element.natural.SentenceAnalyzer.prototype.toString)
1.  [function <span class="apidocSignatureSpan">natural.SentenceAnalyzer.prototype.</span>type (callback)](#apidoc.element.natural.SentenceAnalyzer.prototype.type)

#### [module natural.SentenceTokenizer](#apidoc.module.natural.SentenceTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.</span>SentenceTokenizer ()](#apidoc.element.natural.SentenceTokenizer.SentenceTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.SentenceTokenizer.</span>super_ ()](#apidoc.element.natural.SentenceTokenizer.super_)

#### [module natural.SentenceTokenizer.prototype](#apidoc.module.natural.SentenceTokenizer.prototype)
1.  [function <span class="apidocSignatureSpan">natural.SentenceTokenizer.prototype.</span>tokenize (text)](#apidoc.element.natural.SentenceTokenizer.prototype.tokenize)

#### [module natural.ShortestPathTree](#apidoc.module.natural.ShortestPathTree)
1.  [function <span class="apidocSignatureSpan">natural.</span>ShortestPathTree (digraph, start)](#apidoc.element.natural.ShortestPathTree.ShortestPathTree)

#### [module natural.ShortestPathTree.prototype](#apidoc.module.natural.ShortestPathTree.prototype)
1.  [function <span class="apidocSignatureSpan">natural.ShortestPathTree.prototype.</span>getDistTo (v)](#apidoc.element.natural.ShortestPathTree.prototype.getDistTo)
1.  [function <span class="apidocSignatureSpan">natural.ShortestPathTree.prototype.</span>hasPathTo (v)](#apidoc.element.natural.ShortestPathTree.prototype.hasPathTo)
1.  [function <span class="apidocSignatureSpan">natural.ShortestPathTree.prototype.</span>pathTo (v)](#apidoc.element.natural.ShortestPathTree.prototype.pathTo)
1.  [function <span class="apidocSignatureSpan">natural.ShortestPathTree.prototype.</span>relaxEdge (e)](#apidoc.element.natural.ShortestPathTree.prototype.relaxEdge)
1.  [function <span class="apidocSignatureSpan">natural.ShortestPathTree.prototype.</span>relaxVertex (digraph, vertex, tree)](#apidoc.element.natural.ShortestPathTree.prototype.relaxVertex)

#### [module natural.SoundEx](#apidoc.module.natural.SoundEx)
1.  [function <span class="apidocSignatureSpan">natural.SoundEx.</span>attach ()](#apidoc.element.natural.SoundEx.attach)
1.  [function <span class="apidocSignatureSpan">natural.SoundEx.</span>compare (stringA, stringB)](#apidoc.element.natural.SoundEx.compare)
1.  [function <span class="apidocSignatureSpan">natural.SoundEx.</span>condense (token)](#apidoc.element.natural.SoundEx.condense)
1.  [function <span class="apidocSignatureSpan">natural.SoundEx.</span>padRight0 (token)](#apidoc.element.natural.SoundEx.padRight0)
1.  [function <span class="apidocSignatureSpan">natural.SoundEx.</span>process (token, maxLength)](#apidoc.element.natural.SoundEx.process)
1.  [function <span class="apidocSignatureSpan">natural.SoundEx.</span>transformHum (token)](#apidoc.element.natural.SoundEx.transformHum)
1.  [function <span class="apidocSignatureSpan">natural.SoundEx.</span>transformL (token)](#apidoc.element.natural.SoundEx.transformL)
1.  [function <span class="apidocSignatureSpan">natural.SoundEx.</span>transformLipps (token)](#apidoc.element.natural.SoundEx.transformLipps)
1.  [function <span class="apidocSignatureSpan">natural.SoundEx.</span>transformR (token)](#apidoc.element.natural.SoundEx.transformR)
1.  [function <span class="apidocSignatureSpan">natural.SoundEx.</span>transformThroats (token)](#apidoc.element.natural.SoundEx.transformThroats)
1.  [function <span class="apidocSignatureSpan">natural.SoundEx.</span>transformToungue (token)](#apidoc.element.natural.SoundEx.transformToungue)

#### [module natural.SoundExDM](#apidoc.module.natural.SoundExDM)
1.  [function <span class="apidocSignatureSpan">natural.SoundExDM.</span>attach ()](#apidoc.element.natural.SoundExDM.attach)
1.  [function <span class="apidocSignatureSpan">natural.SoundExDM.</span>compare (stringA, stringB)](#apidoc.element.natural.SoundExDM.compare)
1.  [function <span class="apidocSignatureSpan">natural.SoundExDM.</span>process (word, codeLength)](#apidoc.element.natural.SoundExDM.process)

#### [module natural.Spellcheck](#apidoc.module.natural.Spellcheck)
1.  [function <span class="apidocSignatureSpan">natural.</span>Spellcheck (wordlist)](#apidoc.element.natural.Spellcheck.Spellcheck)

#### [module natural.Spellcheck.prototype](#apidoc.module.natural.Spellcheck.prototype)
1.  [function <span class="apidocSignatureSpan">natural.Spellcheck.prototype.</span>edits (word)](#apidoc.element.natural.Spellcheck.prototype.edits)
1.  [function <span class="apidocSignatureSpan">natural.Spellcheck.prototype.</span>editsWithMaxDistance (word, distance)](#apidoc.element.natural.Spellcheck.prototype.editsWithMaxDistance)
1.  [function <span class="apidocSignatureSpan">natural.Spellcheck.prototype.</span>editsWithMaxDistanceHelper (distanceCounter, distance2edits)](#apidoc.element.natural.Spellcheck.prototype.editsWithMaxDistanceHelper)
1.  [function <span class="apidocSignatureSpan">natural.Spellcheck.prototype.</span>getCorrections (word, maxDistance)](#apidoc.element.natural.Spellcheck.prototype.getCorrections)
1.  [function <span class="apidocSignatureSpan">natural.Spellcheck.prototype.</span>isCorrect (word)](#apidoc.element.natural.Spellcheck.prototype.isCorrect)

#### [module natural.StemmerJa](#apidoc.module.natural.StemmerJa)
1.  [function <span class="apidocSignatureSpan">natural.</span>StemmerJa ()](#apidoc.element.natural.StemmerJa.StemmerJa)

#### [module natural.StemmerJa.prototype](#apidoc.module.natural.StemmerJa.prototype)
1.  [function <span class="apidocSignatureSpan">natural.StemmerJa.prototype.</span>attach ()](#apidoc.element.natural.StemmerJa.prototype.attach)
1.  [function <span class="apidocSignatureSpan">natural.StemmerJa.prototype.</span>isKatakana (str)](#apidoc.element.natural.StemmerJa.prototype.isKatakana)
1.  [function <span class="apidocSignatureSpan">natural.StemmerJa.prototype.</span>stem (token)](#apidoc.element.natural.StemmerJa.prototype.stem)
1.  [function <span class="apidocSignatureSpan">natural.StemmerJa.prototype.</span>stemKatakana (token)](#apidoc.element.natural.StemmerJa.prototype.stemKatakana)
1.  [function <span class="apidocSignatureSpan">natural.StemmerJa.prototype.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.StemmerJa.prototype.tokenizeAndStem)

#### [module natural.TfIdf](#apidoc.module.natural.TfIdf)
1.  [function <span class="apidocSignatureSpan">natural.</span>TfIdf (deserialized)](#apidoc.element.natural.TfIdf.TfIdf)
1.  [function <span class="apidocSignatureSpan">natural.TfIdf.</span>tf (term, document)](#apidoc.element.natural.TfIdf.tf)

#### [module natural.TfIdf.prototype](#apidoc.module.natural.TfIdf.prototype)
1.  [function <span class="apidocSignatureSpan">natural.TfIdf.prototype.</span>addDocument (document, key, restoreCache)](#apidoc.element.natural.TfIdf.prototype.addDocument)
1.  [function <span class="apidocSignatureSpan">natural.TfIdf.prototype.</span>addFileSync (path, encoding, key, restoreCache)](#apidoc.element.natural.TfIdf.prototype.addFileSync)
1.  [function <span class="apidocSignatureSpan">natural.TfIdf.prototype.</span>idf (term, force)](#apidoc.element.natural.TfIdf.prototype.idf)
1.  [function <span class="apidocSignatureSpan">natural.TfIdf.prototype.</span>listTerms (d)](#apidoc.element.natural.TfIdf.prototype.listTerms)
1.  [function <span class="apidocSignatureSpan">natural.TfIdf.prototype.</span>setTokenizer (t)](#apidoc.element.natural.TfIdf.prototype.setTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.TfIdf.prototype.</span>tfidf (terms, d)](#apidoc.element.natural.TfIdf.prototype.tfidf)
1.  [function <span class="apidocSignatureSpan">natural.TfIdf.prototype.</span>tfidfs (terms, callback)](#apidoc.element.natural.TfIdf.prototype.tfidfs)

#### [module natural.TokenizerJa](#apidoc.module.natural.TokenizerJa)
1.  [function <span class="apidocSignatureSpan">natural.</span>TokenizerJa ()](#apidoc.element.natural.TokenizerJa.TokenizerJa)
1.  [function <span class="apidocSignatureSpan">natural.TokenizerJa.</span>super_ ()](#apidoc.element.natural.TokenizerJa.super_)

#### [module natural.TokenizerJa.prototype](#apidoc.module.natural.TokenizerJa.prototype)
1.  [function <span class="apidocSignatureSpan">natural.TokenizerJa.prototype.</span>ctype_ (str)](#apidoc.element.natural.TokenizerJa.prototype.ctype_)
1.  [function <span class="apidocSignatureSpan">natural.TokenizerJa.prototype.</span>removePuncTokens (tokens)](#apidoc.element.natural.TokenizerJa.prototype.removePuncTokens)
1.  [function <span class="apidocSignatureSpan">natural.TokenizerJa.prototype.</span>tokenize (text)](#apidoc.element.natural.TokenizerJa.prototype.tokenize)
1.  [function <span class="apidocSignatureSpan">natural.TokenizerJa.prototype.</span>ts_ (v)](#apidoc.element.natural.TokenizerJa.prototype.ts_)

#### [module natural.TreebankWordTokenizer](#apidoc.module.natural.TreebankWordTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.</span>TreebankWordTokenizer ()](#apidoc.element.natural.TreebankWordTokenizer.TreebankWordTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.TreebankWordTokenizer.</span>super_ ()](#apidoc.element.natural.TreebankWordTokenizer.super_)

#### [module natural.TreebankWordTokenizer.prototype](#apidoc.module.natural.TreebankWordTokenizer.prototype)
1.  [function <span class="apidocSignatureSpan">natural.TreebankWordTokenizer.prototype.</span>tokenize (text)](#apidoc.element.natural.TreebankWordTokenizer.prototype.tokenize)

#### [module natural.Trie](#apidoc.module.natural.Trie)
1.  [function <span class="apidocSignatureSpan">natural.</span>Trie (caseSensitive)](#apidoc.element.natural.Trie.Trie)

#### [module natural.Trie.prototype](#apidoc.module.natural.Trie.prototype)
1.  [function <span class="apidocSignatureSpan">natural.Trie.prototype.</span>addString (string)](#apidoc.element.natural.Trie.prototype.addString)
1.  [function <span class="apidocSignatureSpan">natural.Trie.prototype.</span>addStrings (list)](#apidoc.element.natural.Trie.prototype.addStrings)
1.  [function <span class="apidocSignatureSpan">natural.Trie.prototype.</span>contains (string)](#apidoc.element.natural.Trie.prototype.contains)
1.  [function <span class="apidocSignatureSpan">natural.Trie.prototype.</span>findMatchesOnPath (search)](#apidoc.element.natural.Trie.prototype.findMatchesOnPath)
1.  [function <span class="apidocSignatureSpan">natural.Trie.prototype.</span>findPrefix (search)](#apidoc.element.natural.Trie.prototype.findPrefix)
1.  [function <span class="apidocSignatureSpan">natural.Trie.prototype.</span>getSize ()](#apidoc.element.natural.Trie.prototype.getSize)
1.  [function <span class="apidocSignatureSpan">natural.Trie.prototype.</span>keysWithPrefix (prefix)](#apidoc.element.natural.Trie.prototype.keysWithPrefix)

#### [module natural.WordPunctTokenizer](#apidoc.module.natural.WordPunctTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.</span>WordPunctTokenizer (options)](#apidoc.element.natural.WordPunctTokenizer.WordPunctTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.WordPunctTokenizer.</span>super_ (options)](#apidoc.element.natural.WordPunctTokenizer.super_)

#### [module natural.WordTokenizer](#apidoc.module.natural.WordTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.</span>WordTokenizer (options)](#apidoc.element.natural.WordTokenizer.WordTokenizer)
1.  [function <span class="apidocSignatureSpan">natural.WordTokenizer.</span>super_ (options)](#apidoc.element.natural.WordTokenizer.super_)



# <a name="apidoc.module.natural"></a>[module natural](#apidoc.module.natural)

#### <a name="apidoc.element.natural.AggressiveTokenizer"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizer ()](#apidoc.element.natural.AggressiveTokenizer)
- description and source-code
```javascript
AggressiveTokenizer = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizer.super_"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizer.super_ ()](#apidoc.element.natural.AggressiveTokenizer.super_)
- description and source-code
```javascript
AggressiveTokenizer.super_ = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerEs"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerEs ()](#apidoc.element.natural.AggressiveTokenizerEs)
- description and source-code
```javascript
AggressiveTokenizerEs = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerFa"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerFa ()](#apidoc.element.natural.AggressiveTokenizerFa)
- description and source-code
```javascript
AggressiveTokenizerFa = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerFr"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerFr ()](#apidoc.element.natural.AggressiveTokenizerFr)
- description and source-code
```javascript
AggressiveTokenizerFr = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerIt"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerIt ()](#apidoc.element.natural.AggressiveTokenizerIt)
- description and source-code
```javascript
AggressiveTokenizerIt = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerNl"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerNl ()](#apidoc.element.natural.AggressiveTokenizerNl)
- description and source-code
```javascript
AggressiveTokenizerNl = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerNo"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerNo ()](#apidoc.element.natural.AggressiveTokenizerNo)
- description and source-code
```javascript
AggressiveTokenizerNo = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerPl"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerPl ()](#apidoc.element.natural.AggressiveTokenizerPl)
- description and source-code
```javascript
AggressiveTokenizerPl = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerPt"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerPt ()](#apidoc.element.natural.AggressiveTokenizerPt)
- description and source-code
```javascript
AggressiveTokenizerPt = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerRu"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerRu ()](#apidoc.element.natural.AggressiveTokenizerRu)
- description and source-code
```javascript
AggressiveTokenizerRu = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.BayesClassifier"></a>[function <span class="apidocSignatureSpan">natural.</span>BayesClassifier (stemmer, smoothing)](#apidoc.element.natural.BayesClassifier)
- description and source-code
```javascript
BayesClassifier = function (stemmer, smoothing) {
    var abc = new ApparatusBayesClassifier();
    if (smoothing && isFinite(smoothing)) {
        abc = new ApparatusBayesClassifier(smoothing);
    }
    Classifier.call(this, abc, stemmer);
}
```
- example usage
```shell
...

Two classifiers are currently supported, [Naive Bayes](http://en.wikipedia.org/wiki/Naive_Bayes_classifier) and [logistic regression
](http://en.wikipedia.org/wiki/Logistic_regression).
The following examples use the BayesClassifier class, but the
LogisticRegressionClassifier class could be substituted instead.

'''javascript
var natural = require('natural'),
  classifier = new natural.BayesClassifier();
'''

You can train the classifier on sample text. It will use reasonable defaults to
tokenize and stem the text.

'''javascript
classifier.addDocument('i am long qqqq', 'buy');
...
```

#### <a name="apidoc.element.natural.BayesClassifier.super_"></a>[function <span class="apidocSignatureSpan">natural.</span>BayesClassifier.super_ (classifier, stemmer)](#apidoc.element.natural.BayesClassifier.super_)
- description and source-code
```javascript
BayesClassifier.super_ = function (classifier, stemmer) {
    this.classifier = classifier;
    this.docs = [];
    this.features = {};
    this.stemmer = stemmer || PorterStemmer;
    this.lastAdded = 0;
    this.events = new events.EventEmitter();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.BrillPOSTagger"></a>[function <span class="apidocSignatureSpan">natural.</span>BrillPOSTagger (lexicon, ruleSet)](#apidoc.element.natural.BrillPOSTagger)
- description and source-code
```javascript
function Brill_POS_Tagger(lexicon, ruleSet) {
  this.lexicon = lexicon;
  this.ruleSet = ruleSet;
}
```
- example usage
```shell
...
var base_folder = "some_path/lib/natural/brill_pos_tagger";
var rulesFilename = base_folder + "/data/tr_from_posjs.txt";
var lexiconFilename = base_folder + "/data/lexicon_from_posjs.json";
var defaultCategory = 'N';

var lexicon = new natural.Lexicon(lexiconFilename, defaultCategory);
var rules = new natural.Ruleset(rulesFilename);
var tagger = new natural.BrillPOSTagger(lexicon, rules);

var sentence = ["I", "see", "the", "man", "with", "the", "telescope"];
console.log(JSON.stringify(tagger.tag(sentence)));
'''

### Lexicon
The lexicon is either a JSON file that has the following structure:
...
```

#### <a name="apidoc.element.natural.CaseTokenizer"></a>[function <span class="apidocSignatureSpan">natural.</span>CaseTokenizer ()](#apidoc.element.natural.CaseTokenizer)
- description and source-code
```javascript
CaseTokenizer = function () {
  Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.CountInflector"></a>[function <span class="apidocSignatureSpan">natural.</span>CountInflector ()](#apidoc.element.natural.CountInflector)
- description and source-code
```javascript
CountInflector = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.DiceCoefficient"></a>[function <span class="apidocSignatureSpan">natural.</span>DiceCoefficient (str1, str2)](#apidoc.element.natural.DiceCoefficient)
- description and source-code
```javascript
DiceCoefficient = function (str1, str2) {
  var sanitized_str1 = sanitize(str1);
  var sanitized_str2 = sanitize(str2);
  var pairs1 = wordLetterPairs(sanitized_str1);
  var pairs2 = wordLetterPairs(sanitized_str2);
  var intersection = 0, union = pairs1.length + pairs2.length;
  if (union === 0) {
      if (sanitized_str1 === sanitized_str2) {
          return 1;
      } else {
          return 0;
      }
  } else {
    var i, j, pair1, pair2;
    for (i = 0; i < pairs1.length; i++) {
      pair1 = pairs1[i];
      for (j = 0; j < pairs2.length; j++) {
        pair2 = pairs2[j];
        if (pair1 == pair2) {
          intersection ++;
          delete pairs2[j];
          break;
        }
      }
    }
    return 2 * intersection / union;
  }
}
```
- example usage
```shell
...
1
'''

And Dice's co-efficient:

'''javascript
var natural = require('natural');
console.log(natural.DiceCoefficient('thing', 'thing'));
console.log(natural.DiceCoefficient('not', 'same'));
'''

Output:

'''javascript
1
...
```

#### <a name="apidoc.element.natural.EdgeWeightedDigraph"></a>[function <span class="apidocSignatureSpan">natural.</span>EdgeWeightedDigraph ()](#apidoc.element.natural.EdgeWeightedDigraph)
- description and source-code
```javascript
EdgeWeightedDigraph = function () {
    this.edgesNum = 0;
    this.adj = []; // adjacency list
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.JaroWinklerDistance"></a>[function <span class="apidocSignatureSpan">natural.</span>JaroWinklerDistance (s1, s2, dj)](#apidoc.element.natural.JaroWinklerDistance)
- description and source-code
```javascript
function JaroWinklerDistance(s1, s2, dj) {
		if (s1 == s2) {
				return 1
		}
		else {
		    var jaro;
		    (typeof(dj) == 'undefined')? jaro = distance(s1,s2) : jaro = dj;
		    var p = 0.1; //
		    var l = 0 // length of the matching prefix
		    while(s1[l] == s2[l] && l < 4)
		        l++;
		
		    return jaro + l * p * (1 - jaro);
		}
}
```
- example usage
```shell
...
## String Distance

Natural provides an implementation of the [Jaro–Winkler](http://en.wikipedia.org/wiki/Jaro%E2%80%93Winkler_distance) string distance
 measuring algorithm.
This will return a number between 0 and 1 which tells how closely the strings match (0 = not at all, 1 = exact match):

'''javascript
var natural = require('natural');
console.log(natural.JaroWinklerDistance("dixon","dicksonx"))
console.log(natural.JaroWinklerDistance('not', 'same'));
'''

Output:

'''javascript
0.7466666666666666
...
```

#### <a name="apidoc.element.natural.LevenshteinDistance"></a>[function <span class="apidocSignatureSpan">natural.</span>LevenshteinDistance (source, target, options)](#apidoc.element.natural.LevenshteinDistance)
- description and source-code
```javascript
function LevenshteinDistance(source, target, options) {
    options = options || {};
    if(isNaN(options.insertion_cost)) options.insertion_cost = 1;
    if(isNaN(options.deletion_cost)) options.deletion_cost = 1;
    if(isNaN(options.substitution_cost)) options.substitution_cost = 1;

    var sourceLength = source.length;
    var targetLength = target.length;
    var distanceMatrix = [[0]];

    for (var row =  1; row <= sourceLength; row++) {
        distanceMatrix[row] = [];
        distanceMatrix[row][0] = distanceMatrix[row-1][0] + options.deletion_cost;
    }

    for (var column = 1; column <= targetLength; column++) {
        distanceMatrix[0][column] = distanceMatrix[0][column-1] + options.insertion_cost;
    }

    for (var row = 1; row <= sourceLength; row++) {
        for (var column = 1; column <= targetLength; column++) {
            var costToInsert = distanceMatrix[row][column-1] + options.insertion_cost;
            var costToDelete = distanceMatrix[row-1][column] + options.deletion_cost;

            var sourceElement = source[row-1];
            var targetElement = target[column-1];
            var costToSubstitute = distanceMatrix[row-1][column-1];
            if (sourceElement !== targetElement) {
                costToSubstitute = costToSubstitute + options.substitution_cost;
            }
            distanceMatrix[row][column] = Math.min(costToInsert, costToDelete, costToSubstitute);
        }
    }
    return distanceMatrix[sourceLength][targetLength];
}
```
- example usage
```shell
...
0
'''

Natural also offers support for Levenshtein distances:

'''javascript
var natural = require('natural');
console.log(natural.LevenshteinDistance("ones","onez"));
console.log(natural.LevenshteinDistance('one', 'one'));
'''

Output:

'''javascript
1
...
```

#### <a name="apidoc.element.natural.Lexicon"></a>[function <span class="apidocSignatureSpan">natural.</span>Lexicon (filename, defaultCategory)](#apidoc.element.natural.Lexicon)
- description and source-code
```javascript
function Lexicon(filename, defaultCategory) {
  this.defaultCategory = defaultCategory;
  var that = this;

  // Read lexicon
  try {
    var data = fs.readFileSync(filename, 'utf8');
    if (data[0] === "{") {
      // Lexicon is in JSON format
      that.lexicon = JSON.parse(data);
    }
    else {
      // Lexicon is plain text
      that.parseLexicon(data);
    }
    // console.log('Brill_POS_Tagger.read_lexicon: number of lexicon entries read: ' + Object.keys(that.lexicon).length);
  }
  catch(error) {
    console.error(error);
  }
}
```
- example usage
```shell
...
var natural = require("./lib/natural");

var base_folder = "some_path/lib/natural/brill_pos_tagger";
var rulesFilename = base_folder + "/data/tr_from_posjs.txt";
var lexiconFilename = base_folder + "/data/lexicon_from_posjs.json";
var defaultCategory = 'N';

var lexicon = new natural.Lexicon(lexiconFilename, defaultCategory);
var rules = new natural.Ruleset(rulesFilename);
var tagger = new natural.BrillPOSTagger(lexicon, rules);

var sentence = ["I", "see", "the", "man", "with", "the", "telescope"];
console.log(JSON.stringify(tagger.tag(sentence)));
'''
...
```

#### <a name="apidoc.element.natural.LogisticRegressionClassifier"></a>[function <span class="apidocSignatureSpan">natural.</span>LogisticRegressionClassifier (stemmer)](#apidoc.element.natural.LogisticRegressionClassifier)
- description and source-code
```javascript
LogisticRegressionClassifier = function (stemmer) {
    Classifier.call(this, new ApparatusLogisticRegressionClassifier(), stemmer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.LongestPathTree"></a>[function <span class="apidocSignatureSpan">natural.</span>LongestPathTree (digraph, start)](#apidoc.element.natural.LongestPathTree)
- description and source-code
```javascript
LongestPathTree = function (digraph, start) {
    var _this = this;
    this.edgeTo = [];
    this.distTo = [];
    this.distTo[start] = 0.0;
    this.start = start;
    this.top = new Topological(digraph);
    this.top.order().forEach(function(vertex){
        _this.relaxVertex(digraph, vertex, _this);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NounInflector"></a>[function <span class="apidocSignatureSpan">natural.</span>NounInflector ()](#apidoc.element.natural.NounInflector)
- description and source-code
```javascript
NounInflector = function () {
    this.ambiguous = [
        'bison', 'bream', 'carp', 'chassis', 'cod', 'corps', 'debris', 'deer',
        'diabetes', 'equipment', 'elk', 'fish', 'flounder', 'gallows', 'graffiti',
        'headquarters', 'herpes', 'highjinks', 'homework', 'information',
        'mackerel', 'mews', 'money', 'news', 'rice', 'rabies', 'salmon', 'series',
        'sheep', 'shrimp', 'species', 'swine', 'trout', 'tuna', 'whiting', 'wildebeest'
    ];

    this.customPluralForms = [];
    this.customSingularForms = [];
    this.singularForms = new FormSet();
    this.pluralForms = new FormSet();

    this.attach = attach;

    this.addIrregular("child", "children");
    this.addIrregular("man", "men");
    this.addIrregular("person", "people");
    this.addIrregular("sex", "sexes");
    this.addIrregular("mouse", "mice");
    this.addIrregular("ox", "oxen");
    this.addIrregular("foot", "feet");
    this.addIrregular("tooth", "teeth");
    this.addIrregular("goose", "geese");
    this.addIrregular("ephemeris", "ephemerides");

    // see if it is possible to unify the creation of both the singular and
    // plural regexes or maybe even just have one list. with a complete list
    // of rules it may only be possible for some regular forms, but worth a shot
    this.pluralForms.regularForms.push([/y$/i, 'ies']);
    this.pluralForms.regularForms.push([/ife$/i, 'ives']);
    this.pluralForms.regularForms.push([/(antenn|formul|nebul|vertebr|vit)a$/i, '$1ae']);
    this.pluralForms.regularForms.push([/(octop|vir|radi|nucle|fung|cact|stimul)us$/i, '$1i']);
    this.pluralForms.regularForms.push([/(buffal|tomat|tornad)o$/i, '$1oes']);
    this.pluralForms.regularForms.push([/(sis)$/i, 'ses']);
    this.pluralForms.regularForms.push([/(matr|vert|ind|cort)(ix|ex)$/i, '$1ices']);
    this.pluralForms.regularForms.push([/sses$/i, 'sses']);
    this.pluralForms.regularForms.push([/(x|ch|ss|sh|s|z)$/i, '$1es']);
    this.pluralForms.regularForms.push([/^(?!talis|.*hu)(.*)man$/i, '$1men']);
    this.pluralForms.regularForms.push([/(.*)/i, '$1s']);

    this.singularForms.regularForms.push([/([^v])ies$/i, '$1y']);
    this.singularForms.regularForms.push([/ives$/i, 'ife']);
    this.singularForms.regularForms.push([/(antenn|formul|nebul|vertebr|vit)ae$/i, '$1a']);
    this.singularForms.regularForms.push([/(octop|vir|radi|nucle|fung|cact|stimul)(i)$/i, '$1us']);
    this.singularForms.regularForms.push([/(buffal|tomat|tornad)(oes)$/i, '$1o']);
    this.singularForms.regularForms.push([/(analy|naly|synop|parenthe|diagno|the)ses$/i, '$1sis']);
    this.singularForms.regularForms.push([/(vert|ind|cort)(ices)$/i, '$1ex']);
    // our pluralizer won''t cause this form of appendix (appendicies)
    // but we should handle it
    this.singularForms.regularForms.push([/(matr|append)(ices)$/i, '$1ix']);
    this.singularForms.regularForms.push([/(x|ch|ss|sh|s|z)es$/i, '$1']);
    this.singularForms.regularForms.push([/men$/i, 'man']);
    this.singularForms.regularForms.push([/ss$/i, 'ss']);
    this.singularForms.regularForms.push([/s$/i, '']);

    this.pluralize = function (token) {
        return this.ize(token, this.pluralForms, this.customPluralForms);
    };

    this.singularize = function(token) {
        return this.ize(token, this.singularForms, this.customSingularForms);
    };
}
```
- example usage
```shell
...

### Nouns

Nouns can be pluralized/singularized with a 'NounInflector':

'''javascript
var natural = require('natural'),
nounInflector = new natural.NounInflector();
'''

To pluralize a word (outputs "radii"):

'''javascript
console.log(nounInflector.pluralize('radius'));
'''
...
```

#### <a name="apidoc.element.natural.NounInflector.super_"></a>[function <span class="apidocSignatureSpan">natural.</span>NounInflector.super_ ()](#apidoc.element.natural.NounInflector.super_)
- description and source-code
```javascript
NounInflector.super_ = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NounInflectorFr"></a>[function <span class="apidocSignatureSpan">natural.</span>NounInflectorFr ()](#apidoc.element.natural.NounInflectorFr)
- description and source-code
```javascript
NounInflectorFr = function () {
  // Ambiguous a.k.a. invariant.
  // \@todo Expand this list to be as comprehensive as possible.
  this.ambiguous = [
    // Nouns ending by -s
    'à-peu-près', 'à-propos', 'abattis', 'abcès', 'abois', 'abribus', 'abus',
    'accès', 'acquis', 'adénovirus', 'adonis', 'ados', 'agrès', 'aguets',
    'ailleurs', 'ais', 'albatros', 'albinos', 'alias', 'aloès', 'amaryllis',
    'amas', 'ampélopsis', 'ananas', 'anchois', 'angélus', 'anis', 'anticorps',
    'antihéros', 'antirides', 'anus', 'appas', 'appentis', 'appui-bras',
    'appuie-bras', 'arcanes', 'argus', 'arrérages', 'arrière-pays', 'as',
    'ascaris', 'asparagus', 'atlas', 'atours', 'aurochs', 'autobus',
    'autofocus', 'avant-bras', 'avant-corps', 'avant-propos', 'avers', 'avis',
    'axis', 'barbouillis', 'bas', 'beaujolais', 'beaux-arts', 'biais',
    'bibliobus', 'biceps', 'bicross', 'bien-fonds', 'bloc-notes', 'blockhaus',
    'blocus', 'blues', 'bois', 'bonus', 'bout-dehors', 'bouts-rimés',
    'branle-bas', 'bras', 'brebis', 'bris', 'brise-lames', 'brise-mottes',
    'brûlis', 'buis', 'burnous', 'bus', 'business', 'cabas', 'cacatoès',
    'cacatois', 'cactus', 'cadenas', 'cafouillis', 'caillebotis', 'calvados',
    'cambouis', 'campus', 'canevas', 'cannabis', 'carquois', 'cas',
    'casse-noisettes', 'casse-pieds', 'cassis', 'caucus', 'cens', 'cervelas',
    'chablis', 'chamois', 'chaos', 'chas', 'chasselas', 'châssis',
    'chatouillis', 'chauffe-assiettes', 'chauve-souris', 'chorus', 'choucas',
    'circoncis', 'cirrus', 'clafoutis', 'clapotis', 'cliquetis', 'clos',
    'cochylis', 'colis', 'coloris', 'commis', 'compas', 'compromis',
    'compte-chèques', 'compte-gouttes', 'compte-tours', 'concours', 'confins',
    'congrès', 'consensus', 'contrepoids', 'contresens', 'contretemps',
    'corn flakes', 'corps', 'corps-à-corps', 'corpus', 'cosinus', 'cosmos',
    'coulis', 'coupe-ongles', 'cours', 'court-jus', 'couscous', 'coutelas',
    'crocus', 'croquis', 'cross', 'cubitus', 'cumulus', 'cure-dents',
    'cure-ongles', 'cure-pipes', 'cursus', 'cyclo-cross', 'cyprès', 'dais',
    'damas', 'débarras', 'débours', 'débris', 'décès', 'dedans', 'dehors',
    'delirium tremens', 'demi-gros', 'dépens', 'dessous', 'dessus', 'détritus',
    'deux-mâts', 'deux-pièces', 'deux-points', 'deux-roues', 'deux-temps',
    'dévers', 'devis', 'diplodocus', 'discours', 'dos', 'ébats', 'éboulis',
    'échalas', 'edelweiss', 'élaeis', 'éleis', 'éléphantiasis', 'embarras',
    'empois', 'en-cas', 'encens', 'enclos', 'endos', 'engrais', 'entrelacs',
    'entremets', 'envers', 'épluche-légumes', 'ers', 'espace-temps',
    'essuie-mains', 'eucalyptus', 'ex-libris', 'excès', 'express', 'extrados',
    'faciès', 'fait-divers', 'fatras', 'faux-sens', 'favoris', 'ficus',
    'fier-à-bras', 'finnois', 'florès', 'focus', 'fœtus', 'fois', 'forceps',
    'fouillis', 'fracas', 'frais', 'français', 'franglais', 'frimas',
    'friselis', 'frisottis', 'froncis', 'frottis', 'fucus', 'gâchis', 'galetas',
    'galimatias', 'garde-à-vous', 'garde-corps', 'gargouillis', 'gars',
    'gâte-bois', 'gazouillis', 'génois', 'gibus', 'glacis', 'glas', 'gneiss',
    'gobe-mouches', 'grès', 'gribouillis', 'guet-apens', 'habeas corpus',
    'hachis', 'haras', 'hardes', 'harnais', 'haut-le-corps', 'hautbois',
    'herbe-aux-chats', 'héros', 'herpès', 'hiatus', 'hibiscus', 'hors-concours',
    'hors-pistes', 'hourdis', 'huis-clos', 'humérus', 'humus', 'ibis', 'iléus',
    'indique-fuites', 'infarctus', 'inlandsis', 'insuccès', 'intercours',
    'intrados', 'intrus', 'iris', 'isatis', 'jais', 'jars', 'jeans',
    'jeuconcours', 'judas', 'juliénas', 'jus', 'justaucorps', 'kakatoès',
    'kermès', 'kriss', 'lacis', 'laïus', 'lambris', 'lapis', 'laps', 'lapsus',
    'laquais', 'las', 'lattis', 'lave-mains', 'lavis', 'lèche-bottes',
    'lèche-vitrines', 'legs', 'lias', 'liégeois', 'lilas', 'lis', 'lœss',
    'logis', 'loris', 'lotus', 'louis', 'lupus', 'lys', 'mâchicoulis', 'madras',
    'maïs', 'malappris', 'malus', 'mânes', 'maquis', 'marais', 'maroilles',
    'marquis', 'mas', 'mass-médias', 'matel ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NounInflectorJa"></a>[function <span class="apidocSignatureSpan">natural.</span>NounInflectorJa ()](#apidoc.element.natural.NounInflectorJa)
- description and source-code
```javascript
NounInflectorJa = function () {
  // Ambiguous a.k.a. invariant.
  this.ambiguous = [
    'ともだち', '友だち', '友達', '遊び友達', '飲み友達', '酒飲み友達', '茶飲み友達',
    '学校友達', '女友達', '男友達', '幼友達'
  ];

  this.customPluralForms = [];
  this.customSingularForms = [];
  this.singularForms = new FormSet();
  this.pluralForms = new FormSet();

  this.attach = attach;

  this.addIrregular('神', '神神');
  this.addIrregular('人', '人人');
  this.addIrregular('年', '年年');
  this.addIrregular('月', '月月');
  this.addIrregular('日', '日日');
  this.addIrregular('星', '星星');
  this.addIrregular('島', '島島');
  this.addIrregular('我', '我我');
  this.addIrregular('山', '山山');
  this.addIrregular('国', '国国');
  this.addIrregular('所', '所所');
  this.addIrregular('隅', '隅隅');

<span class="apidocCodeCommentSpan">  /**
   * Notes:
   * -たち exceptions: いたち, おいたち, ついたち, かたち, かおかたち, なりかたち, いでたち, はたち, からたち, なりたち
   * -達 exceptions: 伊達, 男伊達, 栄達, 上意下達, 熟達, 上達, 下意上達, 先達, 送達, 速達, 即日速達, 書留速達, 調達, 通達, 伝達, 到達, 配達, 牛乳配達, 新聞配達, 無料配達, 四通八達, 発達, 未発達, 御用達, 宮内庁御用達, 練達, 闊達
   * -等 exceptions: 一等, 下等, 何等, 均等, 勲等, 高等, 三等, 初等, 上等, 親等, 二親等, 数等, 対等, 中等, 同等, 特等, 二等, 品等, 不等, 平等, 悪平等, 男女平等, 不平等, 優等, 劣等
   */
</span>
  // Pluralize
  this.pluralForms.regularForms.push([/^(.+)$/i, '$1たち']);

  // Singularize
  this.singularForms.regularForms.push([/^(.+)たち$/i, function(a, mask) {
    if (['い', 'おい', 'つい', 'か', 'かおか', 'なりか', 'いで', 'は', 'から',
      'なり'].indexOf(mask) >= 0)
      return mask + 'たち';
    return mask;
  }]);
  this.singularForms.regularForms.push([/^(.+)達$/i, function(a, mask) {
    if (['伊', '伊', '栄', '上意下', '熟', '上', '下意上', '先', '送', '速',
      '即日速', '書留速', '調', '通', '伝', '到', '配', '牛乳配', '新聞配', '無料配',
      '四通八', '発', '未発', '御用', '宮内庁御用', '練', '闊'].indexOf(mask) >= 0)
      return mask + '達';
    return mask;
  }]);  // Singularize nouns ending by -等, but not exceptions.
  this.singularForms.regularForms.push([/^(.+)等$/i, function(a, mask) {
    if (['一', '下', '何', '均', '勲', '高', '三', '初', '親', '二親', '数', '対',
      '中', '同', '特', '二', '品', '不', '平', '悪平', '男女平', '不平', '優',
      '劣'].indexOf(mask) >= 0)
      return mask + '等';
    return mask;
  }]);
  this.singularForms.regularForms.push([/^(人間|わたくし|私|てまえ|手前|野郎|やろう|勇者|がき|ガキ|餓鬼|あくとう|悪党|猫|家来)(共|ども)$/i, '$1']);
  this.singularForms.regularForms.push([/^(神様|先生|あなた|大名|女中|奥様)(方|がた)$/i, '$1']);

  this.pluralize = function(token) {
    return this.ize(token, this.pluralForms, this.customPluralForms);
  };

  this.singularize = function(token) {
    return this.ize(token, this.singularForms, this.customSingularForms);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PresentVerbInflector"></a>[function <span class="apidocSignatureSpan">natural.</span>PresentVerbInflector ()](#apidoc.element.natural.PresentVerbInflector)
- description and source-code
```javascript
PresentVerbInflector = function () {
    this.ambiguous = [
        'will'
    ];

    this.attach = attach;

    this.customPluralForms = [];
    this.customSingularForms = [];
    this.singularForms = new FormSet();
    this.pluralForms = new FormSet();

    this.addIrregular("am", "are");
    this.addIrregular("is", "are");
    this.addIrregular("was", "were");
    this.addIrregular("has", "have");

    this.singularForms.regularForms.push([/ed$/i, 'ed']);
    this.singularForms.regularForms.push([/ss$/i, 'sses']);
    this.singularForms.regularForms.push([/x$/i, 'xes']);
    this.singularForms.regularForms.push([/(h|z|o)$/i, '$1es']);
    this.singularForms.regularForms.push([/$zz/i, 'zzes']);
    this.singularForms.regularForms.push([/([^a|e|i|o|u])y$/i, '$1ies']);
    this.singularForms.regularForms.push([/$/i, 's']);

    this.pluralForms.regularForms.push([/sses$/i, 'ss']);
    this.pluralForms.regularForms.push([/xes$/i, 'x']);
    this.pluralForms.regularForms.push([/([cs])hes$/i, '$1h']);
    this.pluralForms.regularForms.push([/zzes$/i, 'zz']);
    this.pluralForms.regularForms.push([/([^h|z|o|i])es$/i, '$1e']);
    this.pluralForms.regularForms.push([/ies$/i, 'y']);//flies->fly
    this.pluralForms.regularForms.push([/e?s$/i, '']);
}
```
- example usage
```shell
...
### Present Tense Verbs

Present Tense Verbs can be pluralized/singularized with a PresentVerbInflector.
This feature is still experimental as of 0.0.42, so use with caution, and please
provide feedback.

'''javascript
var verbInflector = new natural.PresentVerbInflector();
'''

Outputs "becomes":

'''javascript
console.log(verbInflector.singularize('become'));
'''
...
```

#### <a name="apidoc.element.natural.RegexpTokenizer"></a>[function <span class="apidocSignatureSpan">natural.</span>RegexpTokenizer (options)](#apidoc.element.natural.RegexpTokenizer)
- description and source-code
```javascript
RegexpTokenizer = function (options) {
    var options = options || {};
    this._pattern = options.pattern || this._pattern;
    this.discardEmpty = options.discardEmpty || true;

    // Match and split on GAPS not the actual WORDS
    this._gaps = options.gaps;

    if (this._gaps === undefined) {
        this._gaps = true;
    }
}
```
- example usage
```shell
...
The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
console.log(tokenizer.tokenize("my dog hasn't any fleas."));
// [ 'my', 'dog', 'has', 'n\'t', 'any', 'fleas', '.' ]

tokenizer = new natural.RegexpTokenizer({pattern: /\-/});
console.log(tokenizer.tokenize("flea-dog"));
// [ 'flea', 'dog' ]

tokenizer = new natural.WordPunctTokenizer();
console.log(tokenizer.tokenize("my dog hasn't any fleas."));
// [ 'my',  'dog',  'hasn',  '\'',  't',  'any',  'fleas',  '.' ]
'''
...
```

#### <a name="apidoc.element.natural.RuleSet"></a>[function <span class="apidocSignatureSpan">natural.</span>RuleSet (filename)](#apidoc.element.natural.RuleSet)
- description and source-code
```javascript
function RuleSet(filename) {
  var that = this;

  // Read transformation rules
  try {
    var data = fs.readFileSync(filename, 'utf8');
    this.rules = TF_Parser.parse(data);
    // console.log(this.rules);
    // console.log('Brill_POS_Tagger.read_transformation_rules: number of transformation rules read: ' + this.rules.length);
  }
  catch(error) {
    console.error(error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SentenceAnalyzer"></a>[function <span class="apidocSignatureSpan">natural.</span>SentenceAnalyzer (pos, callback)](#apidoc.element.natural.SentenceAnalyzer)
- description and source-code
```javascript
SentenceAnalyzer = function (pos, callback) {
    this.posObj = pos;
    this.senType = null;
    callback(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SentenceTokenizer"></a>[function <span class="apidocSignatureSpan">natural.</span>SentenceTokenizer ()](#apidoc.element.natural.SentenceTokenizer)
- description and source-code
```javascript
SentenceTokenizer = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.ShortestPathTree"></a>[function <span class="apidocSignatureSpan">natural.</span>ShortestPathTree (digraph, start)](#apidoc.element.natural.ShortestPathTree)
- description and source-code
```javascript
ShortestPathTree = function (digraph, start) {
    var _this = this;
    this.edgeTo = [];
    this.distTo = [];
    this.distTo[start] = 0.0;
    this.start = start;
    this.top = new Topological(digraph);
    this.top.order().forEach(function(vertex){
        _this.relaxVertex(digraph, vertex, _this);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Spellcheck"></a>[function <span class="apidocSignatureSpan">natural.</span>Spellcheck (wordlist)](#apidoc.element.natural.Spellcheck)
- description and source-code
```javascript
function Spellcheck(wordlist) {
    this.trie = new Trie();
    this.trie.addStrings(wordlist);
    this.word2frequency = {};
    for(var i in wordlist) {
        if(!this.word2frequency[wordlist[i]]) {
            this.word2frequency[wordlist[i]] = 0;
        }
        this.word2frequency[wordlist[i]]++;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.StemmerFr"></a>[function <span class="apidocSignatureSpan">natural.</span>StemmerFr ()](#apidoc.element.natural.StemmerFr)
- description and source-code
```javascript
StemmerFr = function () {
   var stemmer = this;

   stemmer.stem = function(token) {
      return token;
   };

   stemmer.tokenizeAndStem = function(text, keepStops) {
      var stemmedTokens = [];

      new Tokenizer().tokenize(text).forEach(function(token) {
         if (keepStops || stopwords.words.indexOf(token) == -1) {
            var resultToken = token.toLowerCase();
            if (resultToken.match(/[a-zâàëéêèïîôûùç0-9]/gi)) {
               resultToken = stemmer.stem(resultToken);
            }
            stemmedTokens.push(resultToken);
         }
      });

      return stemmedTokens;
   };

   stemmer.attach = function() {
      String.prototype.stem = function() {
         return stemmer.stem(this);
      };

      String.prototype.tokenizeAndStem = function(keepStops) {
         return stemmer.tokenizeAndStem(this, keepStops);
      };
   };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.StemmerJa"></a>[function <span class="apidocSignatureSpan">natural.</span>StemmerJa ()](#apidoc.element.natural.StemmerJa)
- description and source-code
```javascript
StemmerJa = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.StemmerPl"></a>[function <span class="apidocSignatureSpan">natural.</span>StemmerPl ()](#apidoc.element.natural.StemmerPl)
- description and source-code
```javascript
StemmerPl = function () {
    var stemmer = this;

    stemmer.stem = function(token) {
        return token;
    };

    stemmer.tokenizeAndStem = function(text, keepStops) {
        var stemmedTokens = [];

        new Tokenizer().tokenize(text).forEach(function(token) {
            if (keepStops || stopwords.words.indexOf(token) == -1) {
                var resultToken = token.toLowerCase();
                if (resultToken.match(new RegExp('[a-zążśźęćńół0-9]+', 'gi'))) {
                    resultToken = stemmer.stem(resultToken);
                }
                stemmedTokens.push(resultToken);
            }
        });

        return stemmedTokens;
    };

    stemmer.attach = function() {
        String.prototype.stem = function() {
            return stemmer.stem(this);
        };

        String.prototype.tokenizeAndStem = function(keepStops) {
            return stemmer.tokenizeAndStem(this, keepStops);
        };
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.TfIdf"></a>[function <span class="apidocSignatureSpan">natural.</span>TfIdf (deserialized)](#apidoc.element.natural.TfIdf)
- description and source-code
```javascript
function TfIdf(deserialized) {
    if(deserialized)
        this.documents = deserialized.documents;
    else
        this.documents = [];

    this._idfCache = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.TokenizerJa"></a>[function <span class="apidocSignatureSpan">natural.</span>TokenizerJa ()](#apidoc.element.natural.TokenizerJa)
- description and source-code
```javascript
TokenizerJa = function () {
  this.chartype_ = [
    [/[〇一二三四五六七八九十百千万億兆]/, 'M'],
    [/[一-鿌〆]/, 'H'],
    [/[ぁ-ゟ]/, 'I'],
    [/[゠-ヿ]/, 'K'],
    [/[a-zA-Z]/, 'A'],
    [/[0-9]/, 'N']
  ];

  this.BIAS__ = -332;
  this.BC1__ = {'HH': 6, 'II': 2461, 'KH': 406, 'OH': -1378};
  this.BC2__ = {'AA': -3267, 'AI': 2744, 'AN': -878, 'HH': -4070, 'HM': -1711, 'HN': 4012, 'HO': 3761, 'IA': 1327, 'IH': -1184, '
II': -1332, 'IK': 1721, 'IO': 5492, 'KI': 3831, 'KK': -8741, 'MH': -3132, 'MK': 3334, 'OO': -2920};
  this.BC3__ = {'HH': 996, 'HI': 626, 'HK': -721, 'HN': -1307, 'HO': -836, 'IH': -301, 'KK': 2762, 'MK': 1079, 'MM': 4034, 'OA': -
1652, 'OH': 266};
  this.BP1__ = {'BB': 295, 'OB': 304, 'OO': -125, 'UB': 352};
  this.BP2__ = {'BO': 60, 'OO': -1762};
  this.BQ1__ = {'BHH': 1150, 'BHM': 1521, 'BII': -1158, 'BIM': 886, 'BMH': 1208, 'BNH': 449, 'BOH': -91, 'BOO': -2597, 'OHI': 451
, 'OIH': -296, 'OKA': 1851, 'OKH': -1020, 'OKK': 904, 'OOO': 2965};
  this.BQ2__ = {'BHH': 118, 'BHI': -1159, 'BHM': 466, 'BIH': -919, 'BKK': -1720, 'BKO': 864, 'OHH': -1139, 'OHM': -181, 'OIH': 153
, 'UHI': -1146};
  this.BQ3__ = {'BHH': -792, 'BHI': 2664, 'BII': -299, 'BKI': 419, 'BMH': 937, 'BMM': 8335, 'BNN': 998, 'BOH': 775, 'OHH': 2174, '
OHM': 439, 'OII': 280, 'OKH': 1798, 'OKI': -793, 'OKO': -2242, 'OMH': -2402, 'OOO': 11699};
  this.BQ4__ = {'BHH': -3895, 'BIH': 3761, 'BII': -4654, 'BIK': 1348, 'BKK': -1806, 'BMI': -3385, 'BOO': -12396, 'OAH': 926, 'OHH
': 266, 'OHK': -2036, 'ONN': -973};
  this.BW1__ = {'，と': 660, '，同': 727, 'B1あ': 1404, 'B1同': 542, '、と': 660, '、同': 727, '｣と': 1682, 'あっ': 1505, 'いう': 1743, 'いっ': -
2055, 'いる': 672, 'うし': -4817, 'うん': 665, 'から': 3472, 'がら': 600, 'こう': -790, 'こと': 2083, 'こん': -1262, 'さら': -4143, 'さん': 4573, 'した':
2641, 'して': 1104, 'すで': -3399, 'そこ': 1977, 'それ': -871, 'たち': 1122, 'ため': 601, 'った': 3463, 'つい': -802, 'てい': 805, 'てき': 1249, 'でき':
1127, 'です': 3445, 'では': 844, 'とい': -4915, 'とみ': 1922, 'どこ': 3887, 'ない': 5713, 'なっ': 3015, 'など': 7379, 'なん': -1113, 'にし': 2468, 'には':
1498, 'にも': 1671, 'に対': -912, 'の一': -501, 'の中': 741, 'ませ': 2448, 'まで': 1711, 'まま': 2600, 'まる': -2155, 'やむ': -1947, 'よっ': -2565, 'れた':
2369, 'れで': -913, 'をし': 1860, 'を見': 731, '亡く': -1886, '京都': 2558, '取り': -2784, '大き': -2604, '大阪': 1497, '平方': -2314, '引き': -1336
, '日本': -195, '本当': -2423, '毎日': -2113, '目指': -724};
  this.BW2__ = {'11': -669, '．．': -11822, '――': -5730, '−−': -13175, 'いう': -1609, 'うか': 2490, 'かし': -1350, 'かも': -602, 'から': -7194
, 'かれ': 4612, 'がい': 853, 'がら': -3198, 'きた': 1941, 'くな': -1597, 'こと': -8392, 'この': -4193, 'させ': 4533, 'され': 13168, 'さん': -3977, 'しい': -
1819, 'しか': -545, 'した': 5078, 'して': 972, 'しな': 939, 'その': -3744, 'たい': -1253, 'たた': -662, 'ただ': -3857, 'たち': -786, 'たと': 1224, 'たは': -
939, 'った': 4589, 'って': 1647, 'っと': -2094, 'てい': 6144, 'てき': 3640, 'てく': 2551, 'ては': -3110, 'ても': -3065, 'でい': 2666, 'でき': -1528, 'でし': -
3828, 'です': -4761, 'でも': -4203, 'とい': 1890, 'とこ': -1746, 'とと': -2279, 'との': 720, 'とみ': 5168, 'とも': -3941, 'ない': -2488, 'なが': -1313
, 'など': -6509, 'なの': 2614, 'なん': 3099, 'にお': -1615, 'にし': 2748, 'にな': 2454, 'によ': -7236, 'に対': -14943, 'に従': -4688, 'に関': -11388
, 'のか': 2093, 'ので': -7059, 'のに': -6041, 'のの': -6125, 'はい': 1073, 'はが': -1033, 'はず': -2532, 'ばれ': 1813, 'まし': -1316, 'まで': -6621, 'まれ':
5409, 'めて': -3153, 'もい': 2230, 'もの': -10713, 'らか': -944, 'らし': -1611, 'らに': -1897, 'りし': 651, 'りま': 1620, 'れた': 4270, 'れて': 849, 'れば':
4114, 'ろう': 6067, 'われ': 7901, 'を通': -11877, 'んだ': 728, 'んな': -4115, '一人': 602, '一方': -1375, '一日': 970, '一部': -1051, '上が': -4479, '会社': -
1116, '出て': 2163, '分の': -7758, '同党': 970, '同日': -913, '大阪': -2471, '委員': -1250, '少な': -1050, '年度': -8669, '年間': -1626, '府県': -2363
, '手権': -1982, '新聞': -4066, '日新': -722, '日本': -7068, '日米': 3372, '曜日': -601, '朝鮮': -2355, '本人': -2697, '東京': -1543, '然と': -1384, '社会': -
1276, '立て': -990, '第に': -1612, '米国': -4268};
  this.BW3__ = {'あた': -2194, 'あり': 719, 'ある': 3846, 'い．': -1185, 'い。': -1185, 'いい': 5308, 'いえ': 2079, 'いく': 3029, 'いた': 2056, 'いっ':
1883, 'いる': 5600, 'いわ': 1527, 'うち': 1117, 'うと': 4798, 'えと': 1454, 'か．': 2857, 'か。': 2857, 'かけ': -743, 'かっ': -4098, 'かに': ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.TreebankWordTokenizer"></a>[function <span class="apidocSignatureSpan">natural.</span>TreebankWordTokenizer ()](#apidoc.element.natural.TreebankWordTokenizer)
- description and source-code
```javascript
TreebankWordTokenizer = function () {
}
```
- example usage
```shell
...
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
console.log(tokenizer.tokenize("my dog hasn't any fleas."));
// [ 'my', 'dog', 'has', 'n\'t', 'any', 'fleas', '.' ]

tokenizer = new natural.RegexpTokenizer({pattern: /\-/});
console.log(tokenizer.tokenize("flea-dog"));
// [ 'flea', 'dog' ]
...
```

#### <a name="apidoc.element.natural.Trie"></a>[function <span class="apidocSignatureSpan">natural.</span>Trie (caseSensitive)](#apidoc.element.natural.Trie)
- description and source-code
```javascript
function Trie(caseSensitive) {
	this.dictionary = {};
	this.$ = false;

	if(typeof caseSensitive === "undefined") {
		caseSensitive = true;
	}

	this.cs = caseSensitive;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.WordNet"></a>[function <span class="apidocSignatureSpan">natural.</span>WordNet (dataDir)](#apidoc.element.natural.WordNet)
- description and source-code
```javascript
function WordNet(dataDir) {

  if (!dataDir) {
    try {
      var WNdb = require('wordnet-db');
    } catch(e) {
      console.error("Please 'npm install wordnet-db' before using WordNet module or specify a dict directory.");
      throw e;
    }
    dataDir = WNdb.path;
  }

  this.nounIndex = new IndexFile(dataDir, 'noun');
  this.verbIndex = new IndexFile(dataDir, 'verb');
  this.adjIndex = new IndexFile(dataDir, 'adj');
  this.advIndex = new IndexFile(dataDir, 'adv');

  this.nounData = new DataFile(dataDir, 'noun');
  this.verbData = new DataFile(dataDir, 'verb');
  this.adjData = new DataFile(dataDir, 'adj');
  this.advData = new DataFile(dataDir, 'adv');

  this.get = get;
  this.lookup = lookup;
  this.lookupFromFiles = lookupFromFiles;
  this.pushResults = pushResults;
  this.loadResultSynonyms = loadResultSynonyms;
  this.loadSynonyms = loadSynonyms;
  this.lookupSynonyms = lookupSynonyms;
  this.getSynonyms = getSynonyms;
  this.getDataFile = getDataFile;
}
```
- example usage
```shell
...

Keep in mind that the WordNet integration is to be considered experimental at this point,
and not production-ready. The API is also subject to change.  For an implementation with vastly increased performance, as well as
 a command-line interface, see [wordpos](https://github.com/moos/wordpos).

Here's an example of looking up definitions for the word "node".

'''javascript
var wordnet = new natural.WordNet();

wordnet.lookup('node', function(results) {
results.forEach(function(result) {
    console.log('------------------------------------');
    console.log(result.synsetOffset);
    console.log(result.pos);
    console.log(result.lemma);
...
```

#### <a name="apidoc.element.natural.WordPunctTokenizer"></a>[function <span class="apidocSignatureSpan">natural.</span>WordPunctTokenizer (options)](#apidoc.element.natural.WordPunctTokenizer)
- description and source-code
```javascript
WordPunctTokenizer = function (options) {
    this._pattern = new RegExp(/(\w+|[а-я0-9_]+|\.|\!|\'|\"")/i);
    RegexpTokenizer.call(this,options)
}
```
- example usage
```shell
...
console.log(tokenizer.tokenize("my dog hasn't any fleas."));
// [ 'my', 'dog', 'has', 'n\'t', 'any', 'fleas', '.' ]

tokenizer = new natural.RegexpTokenizer({pattern: /\-/});
console.log(tokenizer.tokenize("flea-dog"));
// [ 'flea', 'dog' ]

tokenizer = new natural.WordPunctTokenizer();
console.log(tokenizer.tokenize("my dog hasn't any fleas."));
// [ 'my',  'dog',  'hasn',  '\'',  't',  'any',  'fleas',  '.' ]
'''

## String Distance

Natural provides an implementation of the [Jaro–Winkler](http://en.wikipedia.org/wiki/Jaro%E2%80%93Winkler_distance) string distance
 measuring algorithm.
...
```

#### <a name="apidoc.element.natural.WordTokenizer"></a>[function <span class="apidocSignatureSpan">natural.</span>WordTokenizer (options)](#apidoc.element.natural.WordTokenizer)
- description and source-code
```javascript
WordTokenizer = function (options) {
    this._pattern = /[^A-Za-zА-Яа-я0-9_]+/;
    RegexpTokenizer.call(this,options)
}
```
- example usage
```shell
...
## Tokenizers

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
...
```

#### <a name="apidoc.element.natural.normalize"></a>[function <span class="apidocSignatureSpan">natural.</span>normalize (tokens)](#apidoc.element.natural.normalize)
- description and source-code
```javascript
normalize = function (tokens) {
	if(typeof tokens === "string") {
		tokens = [tokens];
	}
        var results = [];
	var rule_count = rules.length;
	var num_tokens = tokens.length;
        var i, token, r, rule;

        for (i = 0; i < num_tokens; i++) {
            token = tokens[i];
            // Check the conversion table
            if (conversionTable[token.toLowerCase()]) {
                results = results.concat(conversionTable[token.toLowerCase()].split(/\W+/));
            }

            // Apply the rules
            else {
                var matched = false;
                for ( r = 0; r < rule_count; r++) {
                    rule = rules[r];
                    if (token.match(rule.regex)) {
                        results = results.concat(token.replace(rule.regex, rule.output).split(/\W+/));
                        matched = true;
                        break;
                    }
                }
                if (!matched) {
                    results.push(token);
                }
            }
        }

	return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.normalize_ja"></a>[function <span class="apidocSignatureSpan">natural.</span>normalize_ja (str)](#apidoc.element.natural.normalize_ja)
- description and source-code
```javascript
normalize_ja = function (str) {
  // Replace repeat characters.
  str = str
    .replace(/(..)々々/g, '$1$1')
    .replace(/(.)々/g, '$1$1');

  str = converters.normalize(str);
  str = converters.fixFullwidthKana(str);

  // Replace composite symbols.
  str = fixCompositeSymbols(str);

  return str;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.removeDiacritics"></a>[function <span class="apidocSignatureSpan">natural.</span>removeDiacritics (str)](#apidoc.element.natural.removeDiacritics)
- description and source-code
```javascript
removeDiacritics = function (str) {
	var rules = diacriticsRemovalMap;
	for (var i = 0; i < rules.length; i++) {
		str = str.replace(rules[i].letters, rules[i].base);
	}
	return str;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.transliterate_ja"></a>[function <span class="apidocSignatureSpan">natural.</span>transliterate_ja (str)](#apidoc.element.natural.transliterate_ja)
- description and source-code
```javascript
transliterate_ja = function (str) {
  str = replace1(str);

  str = str
    .replace(/ッ(?=[ン])/g, 'n')// KATAKANA LETTER SMALL TU
    .replace(/っ(?=[ん])/g, 'n')// HIRAGANA LETTER SMALL TU
    .replace(/ン(?=[バビブベボパピプペポマミムメモ])/g, 'm')// KATAKANA LETTER N
    .replace(/ん(?=[ばびぶべぼぱぴぷぺぽまみむめも])/g, 'm')// HIRAGANA LETTER N
    .replace(/ン(?=[ヤユヨアイウエオ])/g, "n'")// KATAKANA LETTER N
    .replace(/ん(?=[やゆよあいうえお])/g, "n'");// HIRAGANA LETTER N
  str = str
    .replace(/ッ(?=[カキクケコ])/g, 'k')// KATAKANA LETTER SMALL TU
    .replace(/っ(?=[かきくけこ])/g, 'k')// HIRAGANA LETTER SMALL TU
    .replace(/ッ(?=[ガギグゲゴ])/g, 'g')// KATAKANA LETTER SMALL TU
    .replace(/っ(?=[がぎぐげご])/g, 'g')// HIRAGANA LETTER SMALL TU
    .replace(/ッ(?=[サシスセソ])/g, 's')// KATAKANA LETTER SMALL TU
    .replace(/っ(?=[さしすせそ])/g, 's')// HIRAGANA LETTER SMALL TU
    .replace(/ッ(?=[ザズゼゾ])/g, 'z')// KATAKANA LETTER SMALL TU
    .replace(/っ(?=[ざずぜぞ])/g, 'z')// HIRAGANA LETTER SMALL TU
    .replace(/ッ(?=[ジ])/g, 'j')// KATAKANA LETTER SMALL TU
    .replace(/っ(?=[じ])/g, 'j')// HIRAGANA LETTER SMALL TU
    .replace(/ッ(?=[タチツテト])/g, 't')// KATAKANA LETTER SMALL TU
    .replace(/っ(?=[たちつてと])/g, 't')// HIRAGANA LETTER SMALL TU
    .replace(/ッ(?=[ダヂヅデド])/g, 't')// KATAKANA LETTER SMALL TU
    .replace(/っ(?=[だぢづでど])/g, 't')// HIRAGANA LETTER SMALL TU
    .replace(/ッ(?=[ハヒヘホ])/g, 'h')// KATAKANA LETTER SMALL TU
    .replace(/っ(?=[はひへほ])/g, 'h')// HIRAGANA LETTER SMALL TU
    .replace(/ッ(?=[フ])/g, 'f')// KATAKANA LETTER SMALL TU
    .replace(/っ(?=[ふ])/g, 'f')// HIRAGANA LETTER SMALL TU
    .replace(/ッ(?=[バビブベボ])/g, 'b')// KATAKANA LETTER SMALL TU
    .replace(/っ(?=[ばびぶべぼ])/g, 'b')// HIRAGANA LETTER SMALL TU
    .replace(/ッ(?=[パピプペポ])/g, 'p')// KATAKANA LETTER SMALL TU
    .replace(/っ(?=[ぱぴぷぺぽ])/g, 'p')// HIRAGANA LETTER SMALL TU
    .replace(/ッ(?=[ラリルレロ])/g, 'r')// KATAKANA LETTER SMALL TU
    .replace(/っ(?=[らりるれろ])/g, 'r');// HIRAGANA LETTER SMALL TU

  str = replace2(str);
  str = replace3(str);

  str = str
    .replace(/(ッ|っ)\B/g, 't');// FINAL KATAKANA LETTER SMALL TU

  return str;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizer"></a>[module natural.AggressiveTokenizer](#apidoc.module.natural.AggressiveTokenizer)

#### <a name="apidoc.element.natural.AggressiveTokenizer.AggressiveTokenizer"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizer ()](#apidoc.element.natural.AggressiveTokenizer.AggressiveTokenizer)
- description and source-code
```javascript
AggressiveTokenizer = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizer.super_"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizer.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizer.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizer.prototype"></a>[module natural.AggressiveTokenizer.prototype](#apidoc.module.natural.AggressiveTokenizer.prototype)

#### <a name="apidoc.element.natural.AggressiveTokenizer.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizer.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizer.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (text) {
    // break a string up into an array of tokens by anything non-word
    return this.trim(text.split(/\W+/));
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```



# <a name="apidoc.module.natural.AggressiveTokenizer.super_"></a>[module natural.AggressiveTokenizer.super_](#apidoc.module.natural.AggressiveTokenizer.super_)

#### <a name="apidoc.element.natural.AggressiveTokenizer.super_.super_"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizer.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizer.super_.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizer.super_.prototype"></a>[module natural.AggressiveTokenizer.super_.prototype](#apidoc.module.natural.AggressiveTokenizer.super_.prototype)

#### <a name="apidoc.element.natural.AggressiveTokenizer.super_.prototype.attach"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizer.super_.prototype.</span>attach ()](#apidoc.element.natural.AggressiveTokenizer.super_.prototype.attach)
- description and source-code
```javascript
attach = function () {
  var self = this;

  String.prototype.tokenize = function() {
    return self.tokenize(this);
  }
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.AggressiveTokenizer.super_.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizer.super_.prototype.</span>tokenize ()](#apidoc.element.natural.AggressiveTokenizer.super_.prototype.tokenize)
- description and source-code
```javascript
tokenize = function () {}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```

#### <a name="apidoc.element.natural.AggressiveTokenizer.super_.prototype.trim"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizer.super_.prototype.</span>trim (array)](#apidoc.element.natural.AggressiveTokenizer.super_.prototype.trim)
- description and source-code
```javascript
trim = function (array) {
  while (array[array.length - 1] == '')
    array.pop();

  while (array[0] == '')
    array.shift();

  return array;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizerEs"></a>[module natural.AggressiveTokenizerEs](#apidoc.module.natural.AggressiveTokenizerEs)

#### <a name="apidoc.element.natural.AggressiveTokenizerEs.AggressiveTokenizerEs"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerEs ()](#apidoc.element.natural.AggressiveTokenizerEs.AggressiveTokenizerEs)
- description and source-code
```javascript
AggressiveTokenizerEs = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerEs.super_"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerEs.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerEs.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizerEs.prototype"></a>[module natural.AggressiveTokenizerEs.prototype](#apidoc.module.natural.AggressiveTokenizerEs.prototype)

#### <a name="apidoc.element.natural.AggressiveTokenizerEs.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerEs.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerEs.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (text) {
    // break a string up into an array of tokens by anything non-word
    return this.trim(text.split(/[^a-zA-Zá-úÁ-ÚñÑüÜ]+/));
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```



# <a name="apidoc.module.natural.AggressiveTokenizerFa"></a>[module natural.AggressiveTokenizerFa](#apidoc.module.natural.AggressiveTokenizerFa)

#### <a name="apidoc.element.natural.AggressiveTokenizerFa.AggressiveTokenizerFa"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerFa ()](#apidoc.element.natural.AggressiveTokenizerFa.AggressiveTokenizerFa)
- description and source-code
```javascript
AggressiveTokenizerFa = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerFa.super_"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerFa.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerFa.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizerFa.prototype"></a>[module natural.AggressiveTokenizerFa.prototype](#apidoc.module.natural.AggressiveTokenizerFa.prototype)

#### <a name="apidoc.element.natural.AggressiveTokenizerFa.prototype.clearEmptyString"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerFa.prototype.</span>clearEmptyString (array)](#apidoc.element.natural.AggressiveTokenizerFa.prototype.clearEmptyString)
- description and source-code
```javascript
clearEmptyString = function (array) {
	return array.filter(function(a) {
		return a != '';
	});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerFa.prototype.clearText"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerFa.prototype.</span>clearText (text)](#apidoc.element.natural.AggressiveTokenizerFa.prototype.clearText)
- description and source-code
```javascript
clearText = function (text) {
	return text.replace(new RegExp('\.\:\+\-\=\(\)\"\'\!\?\،\,\؛\;', 'g'), ' ');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerFa.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerFa.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerFa.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (text) {
    // break a string up into an array of tokens by anything non-word
    text = this.clearText(text);
    return this.clearEmptyString(text.split(/\s+/));
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```



# <a name="apidoc.module.natural.AggressiveTokenizerFr"></a>[module natural.AggressiveTokenizerFr](#apidoc.module.natural.AggressiveTokenizerFr)

#### <a name="apidoc.element.natural.AggressiveTokenizerFr.AggressiveTokenizerFr"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerFr ()](#apidoc.element.natural.AggressiveTokenizerFr.AggressiveTokenizerFr)
- description and source-code
```javascript
AggressiveTokenizerFr = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerFr.super_"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerFr.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerFr.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizerFr.prototype"></a>[module natural.AggressiveTokenizerFr.prototype](#apidoc.module.natural.AggressiveTokenizerFr.prototype)

#### <a name="apidoc.element.natural.AggressiveTokenizerFr.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerFr.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerFr.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (text) {
    // break a string up into an array of tokens by anything non-word
    return this.trim(text.split(/[^a-z0-9äâàéèëêïîöôùüûœç]+/i));
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```



# <a name="apidoc.module.natural.AggressiveTokenizerIt"></a>[module natural.AggressiveTokenizerIt](#apidoc.module.natural.AggressiveTokenizerIt)

#### <a name="apidoc.element.natural.AggressiveTokenizerIt.AggressiveTokenizerIt"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerIt ()](#apidoc.element.natural.AggressiveTokenizerIt.AggressiveTokenizerIt)
- description and source-code
```javascript
AggressiveTokenizerIt = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerIt.super_"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerIt.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerIt.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizerIt.prototype"></a>[module natural.AggressiveTokenizerIt.prototype](#apidoc.module.natural.AggressiveTokenizerIt.prototype)

#### <a name="apidoc.element.natural.AggressiveTokenizerIt.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerIt.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerIt.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (text) {
    // break a string up into an array of tokens by anything non-word
    return this.trim(text.split(/\W+/));
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```



# <a name="apidoc.module.natural.AggressiveTokenizerNl"></a>[module natural.AggressiveTokenizerNl](#apidoc.module.natural.AggressiveTokenizerNl)

#### <a name="apidoc.element.natural.AggressiveTokenizerNl.AggressiveTokenizerNl"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerNl ()](#apidoc.element.natural.AggressiveTokenizerNl.AggressiveTokenizerNl)
- description and source-code
```javascript
AggressiveTokenizerNl = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerNl.super_"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerNl.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerNl.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizerNl.prototype"></a>[module natural.AggressiveTokenizerNl.prototype](#apidoc.module.natural.AggressiveTokenizerNl.prototype)

#### <a name="apidoc.element.natural.AggressiveTokenizerNl.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerNl.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerNl.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (text) {
    // break a string up into an array of tokens by anything non-word
    return this.trim(text.split(/[^a-zA-Z0-9_']+/));
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```



# <a name="apidoc.module.natural.AggressiveTokenizerNo"></a>[module natural.AggressiveTokenizerNo](#apidoc.module.natural.AggressiveTokenizerNo)

#### <a name="apidoc.element.natural.AggressiveTokenizerNo.AggressiveTokenizerNo"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerNo ()](#apidoc.element.natural.AggressiveTokenizerNo.AggressiveTokenizerNo)
- description and source-code
```javascript
AggressiveTokenizerNo = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerNo.super_"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerNo.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerNo.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizerNo.prototype"></a>[module natural.AggressiveTokenizerNo.prototype](#apidoc.module.natural.AggressiveTokenizerNo.prototype)

#### <a name="apidoc.element.natural.AggressiveTokenizerNo.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerNo.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerNo.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (text) {
    text = normalizer.remove_diacritics(text);

    // break a string up into an array of tokens by anything non-word
    return this.trim(text.split(/[^A-Za-z0-9_æøåÆØÅäÄöÖüÜ]+/));
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```



# <a name="apidoc.module.natural.AggressiveTokenizerPl"></a>[module natural.AggressiveTokenizerPl](#apidoc.module.natural.AggressiveTokenizerPl)

#### <a name="apidoc.element.natural.AggressiveTokenizerPl.AggressiveTokenizerPl"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerPl ()](#apidoc.element.natural.AggressiveTokenizerPl.AggressiveTokenizerPl)
- description and source-code
```javascript
AggressiveTokenizerPl = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerPl.super_"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerPl.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerPl.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizerPl.prototype"></a>[module natural.AggressiveTokenizerPl.prototype](#apidoc.module.natural.AggressiveTokenizerPl.prototype)

#### <a name="apidoc.element.natural.AggressiveTokenizerPl.prototype.clearText"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerPl.prototype.</span>clearText (text)](#apidoc.element.natural.AggressiveTokenizerPl.prototype.clearText)
- description and source-code
```javascript
clearText = function (text) {
	return text.replace(/[^a-zążśźęćńół0-9]/gi, ' ').replace(/[\s\n]+/g, ' ').trim();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerPl.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerPl.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerPl.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (text) {
    // break a string up into an array of tokens by anything non-word
    return this.withoutEmpty(this.clearText(text).split(' '));
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```

#### <a name="apidoc.element.natural.AggressiveTokenizerPl.prototype.withoutEmpty"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerPl.prototype.</span>withoutEmpty (array)](#apidoc.element.natural.AggressiveTokenizerPl.prototype.withoutEmpty)
- description and source-code
```javascript
withoutEmpty = function (array) {
	return array.filter(function(a) {return a;});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizerPt"></a>[module natural.AggressiveTokenizerPt](#apidoc.module.natural.AggressiveTokenizerPt)

#### <a name="apidoc.element.natural.AggressiveTokenizerPt.AggressiveTokenizerPt"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerPt ()](#apidoc.element.natural.AggressiveTokenizerPt.AggressiveTokenizerPt)
- description and source-code
```javascript
AggressiveTokenizerPt = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerPt.super_"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerPt.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerPt.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizerPt.prototype"></a>[module natural.AggressiveTokenizerPt.prototype](#apidoc.module.natural.AggressiveTokenizerPt.prototype)

#### <a name="apidoc.element.natural.AggressiveTokenizerPt.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerPt.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerPt.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (text) {
    // break a string up into an array of tokens by anything non-word
    return this.withoutEmpty(this.trim(text.split(/[^a-zA-Zà-úÀ-Ú]/)));
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```

#### <a name="apidoc.element.natural.AggressiveTokenizerPt.prototype.withoutEmpty"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerPt.prototype.</span>withoutEmpty (array)](#apidoc.element.natural.AggressiveTokenizerPt.prototype.withoutEmpty)
- description and source-code
```javascript
withoutEmpty = function (array) {
	return array.filter(function(a) {return a;});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizerRu"></a>[module natural.AggressiveTokenizerRu](#apidoc.module.natural.AggressiveTokenizerRu)

#### <a name="apidoc.element.natural.AggressiveTokenizerRu.AggressiveTokenizerRu"></a>[function <span class="apidocSignatureSpan">natural.</span>AggressiveTokenizerRu ()](#apidoc.element.natural.AggressiveTokenizerRu.AggressiveTokenizerRu)
- description and source-code
```javascript
AggressiveTokenizerRu = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerRu.super_"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerRu.</span>super_ ()](#apidoc.element.natural.AggressiveTokenizerRu.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.AggressiveTokenizerRu.prototype"></a>[module natural.AggressiveTokenizerRu.prototype](#apidoc.module.natural.AggressiveTokenizerRu.prototype)

#### <a name="apidoc.element.natural.AggressiveTokenizerRu.prototype.clearText"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerRu.prototype.</span>clearText (text)](#apidoc.element.natural.AggressiveTokenizerRu.prototype.clearText)
- description and source-code
```javascript
clearText = function (text) {
	return text.replace(/[^a-zа-яё0-9]/gi, ' ').replace(/[\s\n]+/g, ' ').trim();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.AggressiveTokenizerRu.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerRu.prototype.</span>tokenize (text)](#apidoc.element.natural.AggressiveTokenizerRu.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (text) {
    // break a string up into an array of tokens by anything non-word
    return this.withoutEmpty(this.clearText(text).split(' '));
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```

#### <a name="apidoc.element.natural.AggressiveTokenizerRu.prototype.withoutEmpty"></a>[function <span class="apidocSignatureSpan">natural.AggressiveTokenizerRu.prototype.</span>withoutEmpty (array)](#apidoc.element.natural.AggressiveTokenizerRu.prototype.withoutEmpty)
- description and source-code
```javascript
withoutEmpty = function (array) {
	return array.filter(function(a) {return a;});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.BayesClassifier"></a>[module natural.BayesClassifier](#apidoc.module.natural.BayesClassifier)

#### <a name="apidoc.element.natural.BayesClassifier.BayesClassifier"></a>[function <span class="apidocSignatureSpan">natural.</span>BayesClassifier (stemmer, smoothing)](#apidoc.element.natural.BayesClassifier.BayesClassifier)
- description and source-code
```javascript
BayesClassifier = function (stemmer, smoothing) {
    var abc = new ApparatusBayesClassifier();
    if (smoothing && isFinite(smoothing)) {
        abc = new ApparatusBayesClassifier(smoothing);
    }
    Classifier.call(this, abc, stemmer);
}
```
- example usage
```shell
...

Two classifiers are currently supported, [Naive Bayes](http://en.wikipedia.org/wiki/Naive_Bayes_classifier) and [logistic regression
](http://en.wikipedia.org/wiki/Logistic_regression).
The following examples use the BayesClassifier class, but the
LogisticRegressionClassifier class could be substituted instead.

'''javascript
var natural = require('natural'),
  classifier = new natural.BayesClassifier();
'''

You can train the classifier on sample text. It will use reasonable defaults to
tokenize and stem the text.

'''javascript
classifier.addDocument('i am long qqqq', 'buy');
...
```

#### <a name="apidoc.element.natural.BayesClassifier.load"></a>[function <span class="apidocSignatureSpan">natural.BayesClassifier.</span>load (filename, stemmer, callback)](#apidoc.element.natural.BayesClassifier.load)
- description and source-code
```javascript
function load(filename, stemmer, callback) {
    Classifier.load(filename, function(err, classifier) {
        if (err) {
            callback(err);
        }
        else {
            callback(err, restore(classifier, stemmer));
        }
    });
}
```
- example usage
```shell
...
    // the classifier is saved to the classifier.json file!
});
'''

To recall from the classifier.json saved above:

'''javascript
natural.BayesClassifier.load('classifier.json', null, function(err, classifier) {
    console.log(classifier.classify('long SUNW'));
    console.log(classifier.classify('short SUNW'));
});
'''

A classifier can also be serialized and deserialized like so:
...
```

#### <a name="apidoc.element.natural.BayesClassifier.restore"></a>[function <span class="apidocSignatureSpan">natural.BayesClassifier.</span>restore (classifier, stemmer)](#apidoc.element.natural.BayesClassifier.restore)
- description and source-code
```javascript
function restore(classifier, stemmer) {
    classifier = Classifier.restore(classifier, stemmer);
    classifier.__proto__ = BayesClassifier.prototype;
    classifier.classifier = ApparatusBayesClassifier.restore(classifier.classifier);

    return classifier;
}
```
- example usage
```shell
...
var classifier = new natural.BayesClassifier();
classifier.addDocument(['sell', 'gold'], 'sell');
classifier.addDocument(['buy', 'silver'], 'buy');

// serialize
var raw = JSON.stringify(classifier);
// deserialize
var restoredClassifier = natural.BayesClassifier.restore(JSON.parse(raw));
console.log(restoredClassifier.classify('i should sell that'));
'''

## Phonetics

Phonetic matching (sounds-like) matching can be done with the [SoundEx](http://en.wikipedia.org/wiki/Soundex),
[Metaphone](http://en.wikipedia.org/wiki/Metaphone) or [DoubleMetaphone](http://en.wikipedia.org/wiki/Metaphone#Double_Metaphone
) algorithms
...
```

#### <a name="apidoc.element.natural.BayesClassifier.super_"></a>[function <span class="apidocSignatureSpan">natural.BayesClassifier.</span>super_ (classifier, stemmer)](#apidoc.element.natural.BayesClassifier.super_)
- description and source-code
```javascript
super_ = function (classifier, stemmer) {
    this.classifier = classifier;
    this.docs = [];
    this.features = {};
    this.stemmer = stemmer || PorterStemmer;
    this.lastAdded = 0;
    this.events = new events.EventEmitter();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.BayesClassifier.super_"></a>[module natural.BayesClassifier.super_](#apidoc.module.natural.BayesClassifier.super_)

#### <a name="apidoc.element.natural.BayesClassifier.super_.super_"></a>[function <span class="apidocSignatureSpan">natural.BayesClassifier.</span>super_ (classifier, stemmer)](#apidoc.element.natural.BayesClassifier.super_.super_)
- description and source-code
```javascript
super_ = function (classifier, stemmer) {
    this.classifier = classifier;
    this.docs = [];
    this.features = {};
    this.stemmer = stemmer || PorterStemmer;
    this.lastAdded = 0;
    this.events = new events.EventEmitter();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.BayesClassifier.super_.load"></a>[function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.</span>load (filename, callback)](#apidoc.element.natural.BayesClassifier.super_.load)
- description and source-code
```javascript
function load(filename, callback) {
    var fs = require('fs');

    fs.readFile(filename, 'utf8', function(err, data) {
        var classifier;

        if(!err) {
            classifier = JSON.parse(data);
        }

        if(callback)
            callback(err, classifier);
    });
}
```
- example usage
```shell
...
    // the classifier is saved to the classifier.json file!
});
'''

To recall from the classifier.json saved above:

'''javascript
natural.BayesClassifier.load('classifier.json', null, function(err, classifier) {
    console.log(classifier.classify('long SUNW'));
    console.log(classifier.classify('short SUNW'));
});
'''

A classifier can also be serialized and deserialized like so:
...
```

#### <a name="apidoc.element.natural.BayesClassifier.super_.restore"></a>[function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.</span>restore (classifier, stemmer)](#apidoc.element.natural.BayesClassifier.super_.restore)
- description and source-code
```javascript
function restore(classifier, stemmer) {
    classifier.stemmer = stemmer || PorterStemmer;
    classifier.events = new events.EventEmitter();
    return classifier;
}
```
- example usage
```shell
...
var classifier = new natural.BayesClassifier();
classifier.addDocument(['sell', 'gold'], 'sell');
classifier.addDocument(['buy', 'silver'], 'buy');

// serialize
var raw = JSON.stringify(classifier);
// deserialize
var restoredClassifier = natural.BayesClassifier.restore(JSON.parse(raw));
console.log(restoredClassifier.classify('i should sell that'));
'''

## Phonetics

Phonetic matching (sounds-like) matching can be done with the [SoundEx](http://en.wikipedia.org/wiki/Soundex),
[Metaphone](http://en.wikipedia.org/wiki/Metaphone) or [DoubleMetaphone](http://en.wikipedia.org/wiki/Metaphone#Double_Metaphone
) algorithms
...
```



# <a name="apidoc.module.natural.BayesClassifier.super_.prototype"></a>[module natural.BayesClassifier.super_.prototype](#apidoc.module.natural.BayesClassifier.super_.prototype)

#### <a name="apidoc.element.natural.BayesClassifier.super_.prototype.addDocument"></a>[function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>addDocument (text, classification)](#apidoc.element.natural.BayesClassifier.super_.prototype.addDocument)
- description and source-code
```javascript
function addDocument(text, classification) {

    // Ignore further processing if classification is undefined
    if(typeof classification === 'undefined') return;

    // If classification is type of string then make sure it's dosen't have blank space at both end
    if(typeof classification === 'string'){
      classification = classification.trim();
    }

    if(typeof text === 'string')
	text = this.stemmer.tokenizeAndStem(text);

    if(text.length === 0) {
        // ignore empty documents
        return;
    }

    this.docs.push({
	label: classification,
	text: text
    });

    for (var i = 0; i < text.length; i++) {
        var token = text[i];
        this.features[token] = (this.features[token] || 0) + 1;
    }
}
```
- example usage
```shell
...
  classifier = new natural.BayesClassifier();
'''

You can train the classifier on sample text. It will use reasonable defaults to
tokenize and stem the text.

'''javascript
classifier.addDocument('i am long qqqq', 'buy');
classifier.addDocument('buy the q\'s', 'buy');
classifier.addDocument('short gold', 'sell');
classifier.addDocument('sell gold', 'sell');

classifier.train();
'''
...
```

#### <a name="apidoc.element.natural.BayesClassifier.super_.prototype.classify"></a>[function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>classify (observation)](#apidoc.element.natural.BayesClassifier.super_.prototype.classify)
- description and source-code
```javascript
function classify(observation) {
    return this.classifier.classify(this.textToFeatures(observation));
}
```
- example usage
```shell
...

classifier.train();
'''

Outputs "sell"

'''javascript
console.log(classifier.classify('i am short silver'));
'''

Outputs "buy"

'''javascript
console.log(classifier.classify('i am long copper'));
'''
...
```

#### <a name="apidoc.element.natural.BayesClassifier.super_.prototype.getClassifications"></a>[function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>getClassifications (observation)](#apidoc.element.natural.BayesClassifier.super_.prototype.getClassifications)
- description and source-code
```javascript
function getClassifications(observation) {
    return this.classifier.getClassifications(this.textToFeatures(observation));
}
```
- example usage
```shell
...
[ { label: 'buy', value: 0.39999999999999997 },
  { label: 'sell', value: 0.19999999999999998 } ]
'''

From this:

'''javascript
console.log(classifier.getClassifications('i am long copper'));
'''

The classifier can also be trained with and can classify arrays of tokens, strings, or
any mixture of the two. Arrays let you use entirely custom data with your own
tokenization/stemming, if you choose to implement it.

'''javascript
...
```

#### <a name="apidoc.element.natural.BayesClassifier.super_.prototype.removeDocument"></a>[function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>removeDocument (text, classification)](#apidoc.element.natural.BayesClassifier.super_.prototype.removeDocument)
- description and source-code
```javascript
function removeDocument(text, classification) {
  var docs = this.docs
    , doc
    , pos;

  if (typeof text === 'string') {
    text = this.stemmer.tokenizeAndStem(text);
  }

  for (var i = 0, ii = docs.length; i < ii; i++) {
    doc = docs[i];
    if (doc.text.join(' ') == text.join(' ') &&
        doc.label == classification) {
      pos = i;
    }
  }

  // Remove if there's a match
  if (!isNaN(pos)) {
    this.docs.splice(pos, 1);

    for (var i = 0, ii = text.length; i < ii; i++) {
      delete this.features[text[i]];
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.BayesClassifier.super_.prototype.retrain"></a>[function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>retrain ()](#apidoc.element.natural.BayesClassifier.super_.prototype.retrain)
- description and source-code
```javascript
function retrain() {
  this.classifier = new (this.classifier.constructor)();
  this.lastAdded = 0;
  this.train();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.BayesClassifier.super_.prototype.save"></a>[function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>save (filename, callback)](#apidoc.element.natural.BayesClassifier.super_.prototype.save)
- description and source-code
```javascript
function save(filename, callback) {
    var data = JSON.stringify(this);
    var fs = require('fs');
    var classifier = this;
    fs.writeFile(filename, data, 'utf8', function(err) {
        if(callback) {
            callback(err, err ? null : classifier);
        }
    });
}
```
- example usage
```shell
...
       *  }
       */
    });

A classifier can also be persisted and recalled so you can reuse a training

'''javascript
classifier.save('classifier.json', function(err, classifier) {
    // the classifier is saved to the classifier.json file!
});
'''

To recall from the classifier.json saved above:

'''javascript
...
```

#### <a name="apidoc.element.natural.BayesClassifier.super_.prototype.textToFeatures"></a>[function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>textToFeatures (observation)](#apidoc.element.natural.BayesClassifier.super_.prototype.textToFeatures)
- description and source-code
```javascript
function textToFeatures(observation) {
    var features = [];

    if(typeof observation === 'string')
	observation = this.stemmer.tokenizeAndStem(observation);

    for(var feature in this.features) {
        if(observation.indexOf(feature) > -1)
            features.push(1);
        else
            features.push(0);
    }

    return features;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.BayesClassifier.super_.prototype.train"></a>[function <span class="apidocSignatureSpan">natural.BayesClassifier.super_.prototype.</span>train ()](#apidoc.element.natural.BayesClassifier.super_.prototype.train)
- description and source-code
```javascript
function train() {
    var totalDocs = this.docs.length;
    for(var i = this.lastAdded; i < totalDocs; i++) {
        var features = this.textToFeatures(this.docs[i].text);
        this.classifier.addExample(features, this.docs[i].label);
        this.events.emit('trainedWithDocument', {index: i, total: totalDocs, doc: this.docs[i]});
        this.lastAdded++;
    }
    this.events.emit('doneTraining', true);
    this.classifier.train();
}
```
- example usage
```shell
...

'''javascript
classifier.addDocument('i am long qqqq', 'buy');
classifier.addDocument('buy the q\'s', 'buy');
classifier.addDocument('short gold', 'sell');
classifier.addDocument('sell gold', 'sell');

classifier.train();
'''

Outputs "sell"

'''javascript
console.log(classifier.classify('i am short silver'));
'''
...
```



# <a name="apidoc.module.natural.BrillPOSTagger"></a>[module natural.BrillPOSTagger](#apidoc.module.natural.BrillPOSTagger)

#### <a name="apidoc.element.natural.BrillPOSTagger.BrillPOSTagger"></a>[function <span class="apidocSignatureSpan">natural.</span>BrillPOSTagger (lexicon, ruleSet)](#apidoc.element.natural.BrillPOSTagger.BrillPOSTagger)
- description and source-code
```javascript
function Brill_POS_Tagger(lexicon, ruleSet) {
  this.lexicon = lexicon;
  this.ruleSet = ruleSet;
}
```
- example usage
```shell
...
var base_folder = "some_path/lib/natural/brill_pos_tagger";
var rulesFilename = base_folder + "/data/tr_from_posjs.txt";
var lexiconFilename = base_folder + "/data/lexicon_from_posjs.json";
var defaultCategory = 'N';

var lexicon = new natural.Lexicon(lexiconFilename, defaultCategory);
var rules = new natural.Ruleset(rulesFilename);
var tagger = new natural.BrillPOSTagger(lexicon, rules);

var sentence = ["I", "see", "the", "man", "with", "the", "telescope"];
console.log(JSON.stringify(tagger.tag(sentence)));
'''

### Lexicon
The lexicon is either a JSON file that has the following structure:
...
```



# <a name="apidoc.module.natural.BrillPOSTagger.prototype"></a>[module natural.BrillPOSTagger.prototype](#apidoc.module.natural.BrillPOSTagger.prototype)

#### <a name="apidoc.element.natural.BrillPOSTagger.prototype.tag"></a>[function <span class="apidocSignatureSpan">natural.BrillPOSTagger.prototype.</span>tag (sentence)](#apidoc.element.natural.BrillPOSTagger.prototype.tag)
- description and source-code
```javascript
tag = function (sentence) {
  var taggedSentence = new Array(sentence.length);

  var that = this;
  sentence.forEach(function(word, index) {
    taggedSentence[index] = [];
    taggedSentence[index][0] = word;
    var categories = that.lexicon.tagWord(word);
    taggedSentence[index][1] = categories[0];
  });

  // Apply transformation rules
  for (var i = 0, size = sentence.length; i < size; i++) {
    this.ruleSet.rules.forEach(function(rule) {
      rule.apply(taggedSentence, i);
    });
  }
  return(taggedSentence);
}
```
- example usage
```shell
...
var defaultCategory = 'N';

var lexicon = new natural.Lexicon(lexiconFilename, defaultCategory);
var rules = new natural.Ruleset(rulesFilename);
var tagger = new natural.BrillPOSTagger(lexicon, rules);

var sentence = ["I", "see", "the", "man", "with", "the", "telescope"];
console.log(JSON.stringify(tagger.tag(sentence)));
'''

### Lexicon
The lexicon is either a JSON file that has the following structure:
'''javascript
{
"word1": ["cat1"],
...
```



# <a name="apidoc.module.natural.CaseTokenizer"></a>[module natural.CaseTokenizer](#apidoc.module.natural.CaseTokenizer)

#### <a name="apidoc.element.natural.CaseTokenizer.CaseTokenizer"></a>[function <span class="apidocSignatureSpan">natural.</span>CaseTokenizer ()](#apidoc.element.natural.CaseTokenizer.CaseTokenizer)
- description and source-code
```javascript
CaseTokenizer = function () {
  Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.CaseTokenizer.super_"></a>[function <span class="apidocSignatureSpan">natural.CaseTokenizer.</span>super_ ()](#apidoc.element.natural.CaseTokenizer.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.CaseTokenizer.prototype"></a>[module natural.CaseTokenizer.prototype](#apidoc.module.natural.CaseTokenizer.prototype)

#### <a name="apidoc.element.natural.CaseTokenizer.prototype.attach"></a>[function <span class="apidocSignatureSpan">natural.CaseTokenizer.prototype.</span>attach ()](#apidoc.element.natural.CaseTokenizer.prototype.attach)
- description and source-code
```javascript
attach = function () {
  var self = this;

  String.prototype.tokenize = function(preserveApostrophe) {
    return self.tokenize(this, preserveApostrophe);
  }
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.CaseTokenizer.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.CaseTokenizer.prototype.</span>tokenize (text, preserveApostrophe)](#apidoc.element.natural.CaseTokenizer.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (text, preserveApostrophe) {
  var whitelist = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9'];
  var lower = text.toLowerCase();
  var upper = text.toUpperCase();
  var result = '';
  var i;

  for (i = 0; i < lower.length; ++i) {
    if (lower[i] !== upper[i] || whitelist.indexOf(lower[i]) > -1 || (text[i] === '\'' && preserveApostrophe)) {
      result += text[i];
    } else {
      result += ' ';
    }
  }

  return this.trim(result.replace(/\s+/g, ' ').split(' '));
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```



# <a name="apidoc.module.natural.CountInflector"></a>[module natural.CountInflector](#apidoc.module.natural.CountInflector)

#### <a name="apidoc.element.natural.CountInflector.CountInflector"></a>[function <span class="apidocSignatureSpan">natural.</span>CountInflector ()](#apidoc.element.natural.CountInflector.CountInflector)
- description and source-code
```javascript
CountInflector = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.CountInflector.nth"></a>[function <span class="apidocSignatureSpan">natural.CountInflector.</span>nth (i)](#apidoc.element.natural.CountInflector.nth)
- description and source-code
```javascript
function nth(i) {
    return i.toString() + nthForm(i);
}
```
- example usage
```shell
...
'''javascript
var countInflector = natural.CountInflector;
'''

Outputs "1st":

'''javascript
console.log(countInflector.nth(1));
'''

Outputs "111th":

'''javascript
console.log(countInflector.nth(111));
'''
...
```



# <a name="apidoc.module.natural.DoubleMetaphone"></a>[module natural.DoubleMetaphone](#apidoc.module.natural.DoubleMetaphone)

#### <a name="apidoc.element.natural.DoubleMetaphone.attach"></a>[function <span class="apidocSignatureSpan">natural.DoubleMetaphone.</span>attach ()](#apidoc.element.natural.DoubleMetaphone.attach)
- description and source-code
```javascript
attach = function () {
	var phonetic = this;

    String.prototype.soundsLike = function(compareTo) {
        return phonetic.compare(this, compareTo);
    }

    String.prototype.phonetics = function() {
        return phonetic.process(this);
    }
	
    String.prototype.tokenizeAndPhoneticize = function(keepStops) {
        var phoneticizedTokens = [];

        tokenizer.tokenize(this).forEach(function(token) {
            if(keepStops || stopwords.words.indexOf(token) < 0)
                phoneticizedTokens.push(token.phonetics());
        });

        return phoneticizedTokens;
    }
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.DoubleMetaphone.compare"></a>[function <span class="apidocSignatureSpan">natural.DoubleMetaphone.</span>compare (stringA, stringB)](#apidoc.element.natural.DoubleMetaphone.compare)
- description and source-code
```javascript
function compare(stringA, stringB) {
    var encodingsA = process(stringA),
        encodingsB = process(stringB);

    return encodingsA[0] == encodingsB[0] ||
        encodingsA[1] == encodingsB[1];
}
```
- example usage
```shell
...
var wordA = 'phonetics';
var wordB = 'fonetix';
'''

To test the two words to see if they sound alike:

'''javascript
if(metaphone.compare(wordA, wordB))
    console.log('they sound alike!');
'''

The raw phonetics are obtained with 'process()':

'''javascript
console.log(metaphone.process('phonetics'));
...
```

#### <a name="apidoc.element.natural.DoubleMetaphone.isVowel"></a>[function <span class="apidocSignatureSpan">natural.DoubleMetaphone.</span>isVowel (c)](#apidoc.element.natural.DoubleMetaphone.isVowel)
- description and source-code
```javascript
function isVowel(c) {
	return c && c.match(/[aeiouy]/i);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.DoubleMetaphone.process"></a>[function <span class="apidocSignatureSpan">natural.DoubleMetaphone.</span>process (token, maxLength)](#apidoc.element.natural.DoubleMetaphone.process)
- description and source-code
```javascript
function process(token, maxLength) {
	token = token.toUpperCase();
	var primary = '', secondary = '';	
    var pos = 0;
    maxLength == maxLength || 32;

    function subMatch(startOffset, stopOffset, terms) {
        return subMatchAbsolute(pos + startOffset, pos + stopOffset, terms);
    }

    function subMatchAbsolute(startOffset, stopOffset, terms) {
        return terms.indexOf(token.substring(startOffset, stopOffset)) > -1;
    }

    function addSecondary(primaryAppendage, secondaryAppendage) {
    	primary += primaryAppendage;
    	secondary += secondaryAppendage;
    }

    function add(primaryAppendage) {
    	addSecondary(primaryAppendage, primaryAppendage);
    }

    function addCompressedDouble(c, encoded) {
    	if(token[pos + 1] == c)
    		pos++;
    	add(encoded || c);
    }

    function handleC() {

        if(pos >= 1 && !isVowel(token[pos - 2])
                && token[pos - 1] == 'A' && token[pos + 1] == 'H'
                    && (token[pos + 2] != 'I' && token[pos + 2] != 'I')
                        || subMatch(-2, 4, ['BACHER', 'MACHER'])) {
            add('K');
            pos++;
        } else if(pos == 0 && token.substring(1, 6) == 'EASAR') {
            add('S');
            add('S');
            add('R');
            pos += 6;
        } else if(token.substring(pos + 1, pos + 4) == 'HIA') {
            add('K');
            pos++;
        } else if(token[pos + 1] == 'H') {
            if(pos > 0 && token.substring(pos + 2, pos + 4) == 'AE') {
                addSecondary('K', 'X');
                pos++;
            } else if(pos == 0
                        && (subMatch(1, 6, ['HARAC', 'HARIS'])
                            || subMatch(1, 4, ['HOR', 'HUM', 'HIA', 'HEM']))
                        && token.substring(pos + 1, pos + 5) != 'HORE') {
                add('K');
                pos++;
            } else {
                if((subMatchAbsolute(0, 3, ['VAN', 'VON']) || token.substring(0,  3) == 'SCH')
                    || subMatch(-2, 4, ['ORCHES', 'ARCHIT', 'ORCHID'])
                    || subMatch(2, 3, ['T', 'S'])
                    || ((subMatch(-1, 0, ['A', 'O', 'U', 'E']) || pos == 0)
                        && subMatch(2, 3, ['B', 'F', 'H', 'L', 'M', 'N', 'R', 'V', 'W']))) {
                    add('K');
                } else if(pos > 0) {

                    if(token.substring(0, 2) == 'MC') {
                        add('K');
                    } else {
                        addSecondary('X', 'K');
                    }
                } else {
                    add('X');
                }

                pos++;
            }
        } else if(token.substring(pos, pos + 2) == 'CZ'
                && token.substring(pos - 2, pos + 1) != 'WICZ') {
            addSecondary('S', 'X');
            pos++;
        } else if(token.substring(pos, pos + 3) == 'CIA') {
            add('X');
            pos += 2;
        } else if(token[pos + 1] == 'C' && pos != 1 && token[0] != 'M') {
            if(['I', 'E', 'H'].indexOf(token[pos + 2]) > -1
                    && token.substring(pos + 2, pos + 4) != 'HU') {
                if(pos == 1 && token[pos - 1] == 'A'
                        || subMatch(-1, 4, ['UCCEE', 'UCCES'])) {
                    add('KS');
                } else {
                   add('X');
                }

               pos +=2;
            } else {
                add('K');
                pos++;
            }
        } else if(['K', 'G', 'Q'].indexOf(token[pos + 1]) > -1) {
            add('K');
            pos++;
        } else if(['E', 'I', 'Y'].indexOf(token[pos + 1]) > -1) {
            if(subMatch(1, 3, ['IA', 'IE', 'IO'])) {
                addSecondary('S', 'X');
            } else {
                add('S');
            }
            pos++;
        } else {
            add('K');
            if(token[pos + 1] == ' ' && ['C', 'Q', 'G'].indexOf(token[pos + 2])) {
                pos += 2;
            } else if(['C', 'K', 'Q'].indexOf(token[pos + 1]) > -1
                    && !subMatch(1, 3, ['CE', 'CI'])) { ...
```
- example usage
```shell
...
if(metaphone.compare(wordA, wordB))
    console.log('they sound alike!');
'''

The raw phonetics are obtained with 'process()':

'''javascript
console.log(metaphone.process('phonetics'));
'''

A maximum code length can be supplied:

'''javascript
console.log(metaphone.process('phonetics', 3));
'''
...
```



# <a name="apidoc.module.natural.EdgeWeightedDigraph"></a>[module natural.EdgeWeightedDigraph](#apidoc.module.natural.EdgeWeightedDigraph)

#### <a name="apidoc.element.natural.EdgeWeightedDigraph.EdgeWeightedDigraph"></a>[function <span class="apidocSignatureSpan">natural.</span>EdgeWeightedDigraph ()](#apidoc.element.natural.EdgeWeightedDigraph.EdgeWeightedDigraph)
- description and source-code
```javascript
EdgeWeightedDigraph = function () {
    this.edgesNum = 0;
    this.adj = []; // adjacency list
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.EdgeWeightedDigraph.prototype"></a>[module natural.EdgeWeightedDigraph.prototype](#apidoc.module.natural.EdgeWeightedDigraph.prototype)

#### <a name="apidoc.element.natural.EdgeWeightedDigraph.prototype.add"></a>[function <span class="apidocSignatureSpan">natural.EdgeWeightedDigraph.prototype.</span>add (start, end, weight)](#apidoc.element.natural.EdgeWeightedDigraph.prototype.add)
- description and source-code
```javascript
add = function (start, end, weight) {
    var e = new DirectedEdge(start, end, weight);
    this.addEdge(e);
}
```
- example usage
```shell
...
EdgeWeightedDigraph represents a digraph, you can add an edge, get the number vertexes, edges, get all edges and use toString to
 print the Digraph.

initialize a digraph:

'''javascript
var EdgeWeightedDigraph = natural.EdgeWeightedDigraph;
var digraph = new EdgeWeightedDigraph();
digraph.add(5,4,0.35);
digraph.add(5,1,0.32);
digraph.add(1,3,0.29);
digraph.add(6,2,0.40);
digraph.add(3,6,0.52);
digraph.add(6,4,0.93);
'''
the api used is: add(from, to, weight).
...
```

#### <a name="apidoc.element.natural.EdgeWeightedDigraph.prototype.addEdge"></a>[function <span class="apidocSignatureSpan">natural.EdgeWeightedDigraph.prototype.</span>addEdge (e)](#apidoc.element.natural.EdgeWeightedDigraph.prototype.addEdge)
- description and source-code
```javascript
addEdge = function (e) {
    if(!this.adj[e.from()]) {
        this.adj[e.from()] = new Bag();
    }
    this.adj[e.from()].add(e);
    this.edgesNum++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.EdgeWeightedDigraph.prototype.e"></a>[function <span class="apidocSignatureSpan">natural.EdgeWeightedDigraph.prototype.</span>e ()](#apidoc.element.natural.EdgeWeightedDigraph.prototype.e)
- description and source-code
```javascript
e = function () {
    return this.edgesNum;
}
```
- example usage
```shell
...
console.log(digraph.v());
'''
you will get 5.

get the number of edges:

'''javascript
console.log(digraph.e());
'''
you will get 5.



## ShortestPathTree
...
```

#### <a name="apidoc.element.natural.EdgeWeightedDigraph.prototype.edges"></a>[function <span class="apidocSignatureSpan">natural.EdgeWeightedDigraph.prototype.</span>edges ()](#apidoc.element.natural.EdgeWeightedDigraph.prototype.edges)
- description and source-code
```javascript
edges = function () {
    var adj = this.adj;
    var list = new Bag();
    for(var i in adj) {
        adj[i].unpack().forEach(function(item) {
            list.add(item);
        });
    }
    return list.unpack();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.EdgeWeightedDigraph.prototype.getAdj"></a>[function <span class="apidocSignatureSpan">natural.EdgeWeightedDigraph.prototype.</span>getAdj (v)](#apidoc.element.natural.EdgeWeightedDigraph.prototype.getAdj)
- description and source-code
```javascript
getAdj = function (v) {
    if(!this.adj[v]) return [];
    return this.adj[v].unpack();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.EdgeWeightedDigraph.prototype.toString"></a>[function <span class="apidocSignatureSpan">natural.EdgeWeightedDigraph.prototype.</span>toString ()](#apidoc.element.natural.EdgeWeightedDigraph.prototype.toString)
- description and source-code
```javascript
toString = function () {
    var result = [];
    var list = this.edges();
    list.forEach(function(edge) {
        result.push(edge.toString());
    });
    return result.join('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.EdgeWeightedDigraph.prototype.v"></a>[function <span class="apidocSignatureSpan">natural.EdgeWeightedDigraph.prototype.</span>v ()](#apidoc.element.natural.EdgeWeightedDigraph.prototype.v)
- description and source-code
```javascript
v = function () {
    return this.adj.length;
}
```
- example usage
```shell
...
digraph.add(6,4,0.93);
'''
the api used is: add(from, to, weight).

get the number of vertexes:

'''javascript
console.log(digraph.v());
'''
you will get 5.

get the number of edges:

'''javascript
console.log(digraph.e());
...
```



# <a name="apidoc.module.natural.LancasterStemmer"></a>[module natural.LancasterStemmer](#apidoc.module.natural.LancasterStemmer)

#### <a name="apidoc.element.natural.LancasterStemmer.addStopWord"></a>[function <span class="apidocSignatureSpan">natural.LancasterStemmer.</span>addStopWord (stopWord)](#apidoc.element.natural.LancasterStemmer.addStopWord)
- description and source-code
```javascript
addStopWord = function (stopWord) {
    stopwords.words.push(stopWord);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.LancasterStemmer.addStopWords"></a>[function <span class="apidocSignatureSpan">natural.LancasterStemmer.</span>addStopWords (moreStopWords)](#apidoc.element.natural.LancasterStemmer.addStopWords)
- description and source-code
```javascript
addStopWords = function (moreStopWords) {
    stopwords.words = stopwords.words.concat(moreStopWords);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.LancasterStemmer.attach"></a>[function <span class="apidocSignatureSpan">natural.LancasterStemmer.</span>attach ()](#apidoc.element.natural.LancasterStemmer.attach)
- description and source-code
```javascript
attach = function () {
    String.prototype.stem = function() {
        return stemmer.stem(this);
    };

    String.prototype.tokenizeAndStem = function(keepStops) {
        return stemmer.tokenizeAndStem(this, keepStops);
    };
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.LancasterStemmer.removeStopWord"></a>[function <span class="apidocSignatureSpan">natural.LancasterStemmer.</span>removeStopWord (stopWord)](#apidoc.element.natural.LancasterStemmer.removeStopWord)
- description and source-code
```javascript
removeStopWord = function (stopWord) {
    this.removeStopWords([stopWord])
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.LancasterStemmer.removeStopWords"></a>[function <span class="apidocSignatureSpan">natural.LancasterStemmer.</span>removeStopWords (moreStopWords)](#apidoc.element.natural.LancasterStemmer.removeStopWords)
- description and source-code
```javascript
removeStopWords = function (moreStopWords) {
    moreStopWords.forEach(function(stopWord){
        var idx = stopwords.words.indexOf(stopWord);
        if (idx >= 0) {
            stopwords.words.splice(idx, 1);
        }
    });

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.LancasterStemmer.stem"></a>[function <span class="apidocSignatureSpan">natural.LancasterStemmer.</span>stem (token)](#apidoc.element.natural.LancasterStemmer.stem)
- description and source-code
```javascript
stem = function (token) {
    return applyRuleSection(token.toLowerCase(), true);
}
```
- example usage
```shell
...
'''javascript
var natural = require('natural');
'''

This example uses a Porter stemmer. "word" is returned.

'''javascript
console.log(natural.PorterStemmer.stem("words")); // stem a single word
'''

 in Russian:

'''javascript
console.log(natural.PorterStemmerRu.stem("падший"));
'''
...
```

#### <a name="apidoc.element.natural.LancasterStemmer.tokenizeAndStem"></a>[function <span class="apidocSignatureSpan">natural.LancasterStemmer.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.LancasterStemmer.tokenizeAndStem)
- description and source-code
```javascript
tokenizeAndStem = function (text, keepStops) {
    var stemmedTokens = [];
    var lowercaseText = text.toLowerCase();
    var tokens = new Tokenizer().tokenize(lowercaseText);

    if (keepStops) {
        tokens.forEach(function(token) {
            stemmedTokens.push(stemmer.stem(token));
        });
    }

    else {
        tokens.forEach(function(token) {
            if (stopwords.words.indexOf(token) == -1)
                stemmedTokens.push(stemmer.stem(token));
        });
    }

    return stemmedTokens;
}
```
- example usage
```shell
...

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
natural.LancasterStemmer.attach();
...
```



# <a name="apidoc.module.natural.Lexicon"></a>[module natural.Lexicon](#apidoc.module.natural.Lexicon)

#### <a name="apidoc.element.natural.Lexicon.Lexicon"></a>[function <span class="apidocSignatureSpan">natural.</span>Lexicon (filename, defaultCategory)](#apidoc.element.natural.Lexicon.Lexicon)
- description and source-code
```javascript
function Lexicon(filename, defaultCategory) {
  this.defaultCategory = defaultCategory;
  var that = this;

  // Read lexicon
  try {
    var data = fs.readFileSync(filename, 'utf8');
    if (data[0] === "{") {
      // Lexicon is in JSON format
      that.lexicon = JSON.parse(data);
    }
    else {
      // Lexicon is plain text
      that.parseLexicon(data);
    }
    // console.log('Brill_POS_Tagger.read_lexicon: number of lexicon entries read: ' + Object.keys(that.lexicon).length);
  }
  catch(error) {
    console.error(error);
  }
}
```
- example usage
```shell
...
var natural = require("./lib/natural");

var base_folder = "some_path/lib/natural/brill_pos_tagger";
var rulesFilename = base_folder + "/data/tr_from_posjs.txt";
var lexiconFilename = base_folder + "/data/lexicon_from_posjs.json";
var defaultCategory = 'N';

var lexicon = new natural.Lexicon(lexiconFilename, defaultCategory);
var rules = new natural.Ruleset(rulesFilename);
var tagger = new natural.BrillPOSTagger(lexicon, rules);

var sentence = ["I", "see", "the", "man", "with", "the", "telescope"];
console.log(JSON.stringify(tagger.tag(sentence)));
'''
...
```



# <a name="apidoc.module.natural.Lexicon.prototype"></a>[module natural.Lexicon.prototype](#apidoc.module.natural.Lexicon.prototype)

#### <a name="apidoc.element.natural.Lexicon.prototype.parseLexicon"></a>[function <span class="apidocSignatureSpan">natural.Lexicon.prototype.</span>parseLexicon (data)](#apidoc.element.natural.Lexicon.prototype.parseLexicon)
- description and source-code
```javascript
parseLexicon = function (data) {
  // Split into an array of non-empty lines
  var arrayOfLines = data.match(/[^\r\n]+/g);
  this.lexicon = {};
  var that = this;
  arrayOfLines.forEach(function(line) {
    // Split line by whitespace
    var elements = line.trim().split(/\s+/);
    if (elements.length > 0) {
      that.lexicon[elements[0]] = elements.slice(1);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Lexicon.prototype.tagWord"></a>[function <span class="apidocSignatureSpan">natural.Lexicon.prototype.</span>tagWord (word)](#apidoc.element.natural.Lexicon.prototype.tagWord)
- description and source-code
```javascript
tagWord = function (word) {
  var categories = this.lexicon[word];
  if (!categories) {
    categories = this.lexicon[word.toLowerCase()];
  }
  if (!categories) {
    // If not found assign default_category
    categories = [this.defaultCategory];
  }
  return(categories);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.LogisticRegressionClassifier"></a>[module natural.LogisticRegressionClassifier](#apidoc.module.natural.LogisticRegressionClassifier)

#### <a name="apidoc.element.natural.LogisticRegressionClassifier.LogisticRegressionClassifier"></a>[function <span class="apidocSignatureSpan">natural.</span>LogisticRegressionClassifier (stemmer)](#apidoc.element.natural.LogisticRegressionClassifier.LogisticRegressionClassifier)
- description and source-code
```javascript
LogisticRegressionClassifier = function (stemmer) {
    Classifier.call(this, new ApparatusLogisticRegressionClassifier(), stemmer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.LogisticRegressionClassifier.load"></a>[function <span class="apidocSignatureSpan">natural.LogisticRegressionClassifier.</span>load (filename, stemmer, callback)](#apidoc.element.natural.LogisticRegressionClassifier.load)
- description and source-code
```javascript
function load(filename, stemmer, callback) {
    Classifier.load(filename, function(err, classifier) {
        if (err) {
            callback(err);
        }
        else {
            callback(err, restore(classifier, stemmer));
        }
    });
}
```
- example usage
```shell
...
    // the classifier is saved to the classifier.json file!
});
'''

To recall from the classifier.json saved above:

'''javascript
natural.BayesClassifier.load('classifier.json', null, function(err, classifier) {
    console.log(classifier.classify('long SUNW'));
    console.log(classifier.classify('short SUNW'));
});
'''

A classifier can also be serialized and deserialized like so:
...
```

#### <a name="apidoc.element.natural.LogisticRegressionClassifier.restore"></a>[function <span class="apidocSignatureSpan">natural.LogisticRegressionClassifier.</span>restore (classifier, stemmer)](#apidoc.element.natural.LogisticRegressionClassifier.restore)
- description and source-code
```javascript
function restore(classifier, stemmer) {
    classifier = Classifier.restore(classifier, stemmer);
    classifier.__proto__ = LogisticRegressionClassifier.prototype;
    classifier.classifier = ApparatusLogisticRegressionClassifier.restore(classifier.classifier);

    return classifier;
}
```
- example usage
```shell
...
var classifier = new natural.BayesClassifier();
classifier.addDocument(['sell', 'gold'], 'sell');
classifier.addDocument(['buy', 'silver'], 'buy');

// serialize
var raw = JSON.stringify(classifier);
// deserialize
var restoredClassifier = natural.BayesClassifier.restore(JSON.parse(raw));
console.log(restoredClassifier.classify('i should sell that'));
'''

## Phonetics

Phonetic matching (sounds-like) matching can be done with the [SoundEx](http://en.wikipedia.org/wiki/Soundex),
[Metaphone](http://en.wikipedia.org/wiki/Metaphone) or [DoubleMetaphone](http://en.wikipedia.org/wiki/Metaphone#Double_Metaphone
) algorithms
...
```

#### <a name="apidoc.element.natural.LogisticRegressionClassifier.super_"></a>[function <span class="apidocSignatureSpan">natural.LogisticRegressionClassifier.</span>super_ (classifier, stemmer)](#apidoc.element.natural.LogisticRegressionClassifier.super_)
- description and source-code
```javascript
super_ = function (classifier, stemmer) {
    this.classifier = classifier;
    this.docs = [];
    this.features = {};
    this.stemmer = stemmer || PorterStemmer;
    this.lastAdded = 0;
    this.events = new events.EventEmitter();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.LogisticRegressionClassifier.prototype"></a>[module natural.LogisticRegressionClassifier.prototype](#apidoc.module.natural.LogisticRegressionClassifier.prototype)

#### <a name="apidoc.element.natural.LogisticRegressionClassifier.prototype.train"></a>[function <span class="apidocSignatureSpan">natural.LogisticRegressionClassifier.prototype.</span>train ()](#apidoc.element.natural.LogisticRegressionClassifier.prototype.train)
- description and source-code
```javascript
function train() {
    // we need to reset the traning state because logistic regression
    // needs its matricies to have their widths synced, etc.
    this.lastAdded = 0;
    this.classifier = new ApparatusLogisticRegressionClassifier();
    Classifier.prototype.train.call(this);
}
```
- example usage
```shell
...

'''javascript
classifier.addDocument('i am long qqqq', 'buy');
classifier.addDocument('buy the q\'s', 'buy');
classifier.addDocument('short gold', 'sell');
classifier.addDocument('sell gold', 'sell');

classifier.train();
'''

Outputs "sell"

'''javascript
console.log(classifier.classify('i am short silver'));
'''
...
```



# <a name="apidoc.module.natural.LongestPathTree"></a>[module natural.LongestPathTree](#apidoc.module.natural.LongestPathTree)

#### <a name="apidoc.element.natural.LongestPathTree.LongestPathTree"></a>[function <span class="apidocSignatureSpan">natural.</span>LongestPathTree (digraph, start)](#apidoc.element.natural.LongestPathTree.LongestPathTree)
- description and source-code
```javascript
LongestPathTree = function (digraph, start) {
    var _this = this;
    this.edgeTo = [];
    this.distTo = [];
    this.distTo[start] = 0.0;
    this.start = start;
    this.top = new Topological(digraph);
    this.top.order().forEach(function(vertex){
        _this.relaxVertex(digraph, vertex, _this);
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.LongestPathTree.prototype"></a>[module natural.LongestPathTree.prototype](#apidoc.module.natural.LongestPathTree.prototype)

#### <a name="apidoc.element.natural.LongestPathTree.prototype.getDistTo"></a>[function <span class="apidocSignatureSpan">natural.LongestPathTree.prototype.</span>getDistTo (v)](#apidoc.element.natural.LongestPathTree.prototype.getDistTo)
- description and source-code
```javascript
getDistTo = function (v) {
    return this.distTo[v];
}
```
- example usage
```shell
...
digraph is an instance of EdgeWeightedDigraph, the second param is the start vertex of DAG.

### getDistTo(vertex)

Will return the dist to vertex.

'''javascript
console.log(spt.getDistTo(4));
'''
the output will be: 0.35

### hasDistTo(vertex)

'''javascript
console.log(spt.hasDistTo(4));
...
```

#### <a name="apidoc.element.natural.LongestPathTree.prototype.hasPathTo"></a>[function <span class="apidocSignatureSpan">natural.LongestPathTree.prototype.</span>hasPathTo (v)](#apidoc.element.natural.LongestPathTree.prototype.hasPathTo)
- description and source-code
```javascript
hasPathTo = function (v) {
    return !!this.distTo[v];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.LongestPathTree.prototype.pathTo"></a>[function <span class="apidocSignatureSpan">natural.LongestPathTree.prototype.</span>pathTo (v)](#apidoc.element.natural.LongestPathTree.prototype.pathTo)
- description and source-code
```javascript
pathTo = function (v) {
    if (!this.hasPathTo(v)) return [];
    var path = [];
    var edgeTo = this.edgeTo;
    for (var e = edgeTo[v]; !!e; e = edgeTo[e.from()]) {
        path.push(e.to());
    }
    path.push(this.start);
    return path.reverse();
}
```
- example usage
```shell
...
false
'''

### pathTo(vertex)
this will return a shortest path:

'''javascript
console.log(spt.pathTo(4));
'''

output will be:

'''javascript
[5, 4]
'''
...
```

#### <a name="apidoc.element.natural.LongestPathTree.prototype.relaxEdge"></a>[function <span class="apidocSignatureSpan">natural.LongestPathTree.prototype.</span>relaxEdge (e)](#apidoc.element.natural.LongestPathTree.prototype.relaxEdge)
- description and source-code
```javascript
relaxEdge = function (e) {
    var distTo = this.distTo,
        edgeTo = this.edgeTo;
    var v = e.from(), w = e.to();
    if (distTo[w] < distTo[v] + e.weight) {
        distTo[w] = distTo[v] + e.weight;
        edgeTo[w] = e;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.LongestPathTree.prototype.relaxVertex"></a>[function <span class="apidocSignatureSpan">natural.LongestPathTree.prototype.</span>relaxVertex (digraph, vertex, tree)](#apidoc.element.natural.LongestPathTree.prototype.relaxVertex)
- description and source-code
```javascript
relaxVertex = function (digraph, vertex, tree) {
    var distTo = tree.distTo;
    var edgeTo = tree.edgeTo;

    digraph.getAdj(vertex).forEach(function(edge){
        var w = edge.to();
        distTo[w] = distTo[w] || 0.0;
        distTo[vertex] = distTo[vertex] || 0.0;
        if (distTo[w] < distTo[vertex] + edge.weight) {
            // in case of the result of 0.28+0.34 is 0.62000001
            distTo[w] = parseFloat((distTo[vertex] + edge.weight).toFixed(2));
            edgeTo[w] = edge;
        }
    });

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.Metaphone"></a>[module natural.Metaphone](#apidoc.module.natural.Metaphone)

#### <a name="apidoc.element.natural.Metaphone.attach"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>attach ()](#apidoc.element.natural.Metaphone.attach)
- description and source-code
```javascript
attach = function () {
	var phonetic = this;

    String.prototype.soundsLike = function(compareTo) {
        return phonetic.compare(this, compareTo);
    }

    String.prototype.phonetics = function() {
        return phonetic.process(this);
    }
	
    String.prototype.tokenizeAndPhoneticize = function(keepStops) {
        var phoneticizedTokens = [];

        tokenizer.tokenize(this).forEach(function(token) {
            if(keepStops || stopwords.words.indexOf(token) < 0)
                phoneticizedTokens.push(token.phonetics());
        });

        return phoneticizedTokens;
    }
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.Metaphone.cTransform"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>cTransform (token)](#apidoc.element.natural.Metaphone.cTransform)
- description and source-code
```javascript
function cTransform(token) {


    token = token.replace(/([^s]|^)(c)(h)/g, '$1x$3').trim();


    token = token.replace(/cia/g, 'xia');
    token = token.replace(/c(i|e|y)/g, 's$1');
    token = token.replace(/c/g, 'k');

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.compare"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>compare (stringA, stringB)](#apidoc.element.natural.Metaphone.compare)
- description and source-code
```javascript
compare = function (stringA, stringB) {
    return this.process(stringA) == this.process(stringB);
}
```
- example usage
```shell
...
var wordA = 'phonetics';
var wordB = 'fonetix';
'''

To test the two words to see if they sound alike:

'''javascript
if(metaphone.compare(wordA, wordB))
    console.log('they sound alike!');
'''

The raw phonetics are obtained with 'process()':

'''javascript
console.log(metaphone.process('phonetics'));
...
```

#### <a name="apidoc.element.natural.Metaphone.dTransform"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>dTransform (token)](#apidoc.element.natural.Metaphone.dTransform)
- description and source-code
```javascript
function dTransform(token) {
    token = token.replace(/d(ge|gy|gi)/g, 'j$1');
    token = token.replace(/d/g, 't');

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.dedup"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>dedup (token)](#apidoc.element.natural.Metaphone.dedup)
- description and source-code
```javascript
function dedup(token) {
    return token.replace(/([^c])\1/g, '$1');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.dropBafterMAtEnd"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropBafterMAtEnd (token)](#apidoc.element.natural.Metaphone.dropBafterMAtEnd)
- description and source-code
```javascript
function dropBafterMAtEnd(token) {
    return token.replace(/mb$/, 'm');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.dropG"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropG (token)](#apidoc.element.natural.Metaphone.dropG)
- description and source-code
```javascript
function dropG(token) {
    token = token.replace(/gh(^$|[^aeiou])/g, 'h$1');
    token = token.replace(/g(n|ned)$/g, '$1');

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.dropH"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropH (token)](#apidoc.element.natural.Metaphone.dropH)
- description and source-code
```javascript
function dropH(token) {
    return token.replace(/([aeiou])h([^aeiou]|$)/g, '$1$2');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.dropInitialLetters"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropInitialLetters (token)](#apidoc.element.natural.Metaphone.dropInitialLetters)
- description and source-code
```javascript
function dropInitialLetters(token) {
    if(token.match(/^(kn|gn|pn|ae|wr)/))
        return token.substr(1, token.length - 1);

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.dropT"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropT (token)](#apidoc.element.natural.Metaphone.dropT)
- description and source-code
```javascript
function dropT(token) {
    return token.replace(/tch/g, 'ch');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.dropVowels"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropVowels (token)](#apidoc.element.natural.Metaphone.dropVowels)
- description and source-code
```javascript
function dropVowels(token) {
    return token.charAt(0) + token.substr(1, token.length).replace(/[aeiou]/g, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.dropW"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropW (token)](#apidoc.element.natural.Metaphone.dropW)
- description and source-code
```javascript
function dropW(token) {
    return token.replace(/w([^aeiou]|$)/g, '$1');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.dropY"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>dropY (token)](#apidoc.element.natural.Metaphone.dropY)
- description and source-code
```javascript
function dropY(token) {
    return token.replace(/y([^aeiou]|$)/g, '$1');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.process"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>process (token, maxLength)](#apidoc.element.natural.Metaphone.process)
- description and source-code
```javascript
process = function (token, maxLength) {
    maxLength == maxLength || 32;
    token = token.toLowerCase();
    token = dedup(token);
    token = dropInitialLetters(token);
    token = dropBafterMAtEnd(token);
    token = transformCK(token);
    token = cTransform(token);
    token = dTransform(token);
    token = dropG(token);
    token = transformG(token);
    token = dropH(token);
    token = transformPH(token);
    token = transformQ(token);
    token = transformS(token);
    token = transformX(token);
    token = transformT(token);
    token = dropT(token);
    token = transformV(token);
    token = transformWH(token);
    token = dropW(token);
    token = dropY(token);
    token = transformZ(token);
    token = dropVowels(token);

    token.toUpperCase();
    if(token.length >= maxLength)
        token = token.substring(0, maxLength);

    return token.toUpperCase();
}
```
- example usage
```shell
...
if(metaphone.compare(wordA, wordB))
    console.log('they sound alike!');
'''

The raw phonetics are obtained with 'process()':

'''javascript
console.log(metaphone.process('phonetics'));
'''

A maximum code length can be supplied:

'''javascript
console.log(metaphone.process('phonetics', 3));
'''
...
```

#### <a name="apidoc.element.natural.Metaphone.transformCK"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformCK (token)](#apidoc.element.natural.Metaphone.transformCK)
- description and source-code
```javascript
function transformCK(token) {
    return token.replace(/ck/g, 'k');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.transformG"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformG (token)](#apidoc.element.natural.Metaphone.transformG)
- description and source-code
```javascript
function transformG(token) {
    token = token.replace(/gh/g, 'f');
    token = token.replace(/([^g]|^)(g)(i|e|y)/g, '$1j$3');
    token = token.replace(/gg/g, 'g');
    token = token.replace(/g/g, 'k');

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.transformPH"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformPH (token)](#apidoc.element.natural.Metaphone.transformPH)
- description and source-code
```javascript
function transformPH(token) {
    return token.replace(/ph/g, 'f');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.transformQ"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformQ (token)](#apidoc.element.natural.Metaphone.transformQ)
- description and source-code
```javascript
function transformQ(token) {
    return token.replace(/q/g, 'k');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.transformS"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformS (token)](#apidoc.element.natural.Metaphone.transformS)
- description and source-code
```javascript
function transformS(token) {
    return token.replace(/s(h|io|ia)/g, 'x$1');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.transformT"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformT (token)](#apidoc.element.natural.Metaphone.transformT)
- description and source-code
```javascript
function transformT(token) {
    token = token.replace(/t(ia|io)/g, 'x$1');
    token = token.replace(/th/, '0');

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.transformV"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformV (token)](#apidoc.element.natural.Metaphone.transformV)
- description and source-code
```javascript
function transformV(token) {
    return token.replace(/v/g, 'f');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.transformWH"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformWH (token)](#apidoc.element.natural.Metaphone.transformWH)
- description and source-code
```javascript
function transformWH(token) {
    return token.replace(/^wh/, 'w');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.transformX"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformX (token)](#apidoc.element.natural.Metaphone.transformX)
- description and source-code
```javascript
function transformX(token) {
    token = token.replace(/^x/, 's');
    token = token.replace(/x/g, 'ks');
    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Metaphone.transformZ"></a>[function <span class="apidocSignatureSpan">natural.Metaphone.</span>transformZ (token)](#apidoc.element.natural.Metaphone.transformZ)
- description and source-code
```javascript
function transformZ(token) {
    return token.replace(/z/, 's');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.NGrams"></a>[module natural.NGrams](#apidoc.module.natural.NGrams)

#### <a name="apidoc.element.natural.NGrams.bigrams"></a>[function <span class="apidocSignatureSpan">natural.NGrams.</span>bigrams (sequence, startSymbol, endSymbol)](#apidoc.element.natural.NGrams.bigrams)
- description and source-code
```javascript
bigrams = function (sequence, startSymbol, endSymbol) {
    return ngrams(sequence, 2, startSymbol, endSymbol);
}
```
- example usage
```shell
...
'''javascript
var NGrams = natural.NGrams;
'''

### bigrams

'''javascript
console.log(NGrams.bigrams('some words here'));
console.log(NGrams.bigrams(['some',  'words',  'here']));
'''

Both of the above output: '[ [ 'some', 'words' ], [ 'words', 'here' ] ]'

### trigrams
...
```

#### <a name="apidoc.element.natural.NGrams.multrigrams"></a>[function <span class="apidocSignatureSpan">natural.NGrams.</span>multrigrams (sequence, n, startSymbol, endSymbol)](#apidoc.element.natural.NGrams.multrigrams)
- description and source-code
```javascript
multrigrams = function (sequence, n, startSymbol, endSymbol) {
    return ngrams(sequence, n, startSymbol, endSymbol);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NGrams.ngrams"></a>[function <span class="apidocSignatureSpan">natural.NGrams.</span>ngrams (sequence, n, startSymbol, endSymbol)](#apidoc.element.natural.NGrams.ngrams)
- description and source-code
```javascript
ngrams = function (sequence, n, startSymbol, endSymbol) {
    return ngrams(sequence, n, startSymbol, endSymbol);
}
```
- example usage
```shell
...

Both of the above output: '[ [ 'some', 'other', 'words' ],
[ 'other', 'words', 'here' ] ]'

### arbitrary n-grams

'''javascript
console.log(NGrams.ngrams('some other words here for you', 4));
console.log(NGrams.ngrams(['some', 'other', 'words', 'here', 'for',
  'you'], 4));
'''

The above outputs: '[ [ 'some', 'other', 'words', 'here' ],
[ 'other', 'words', 'here', 'for' ],
[ 'words', 'here', 'for', 'you' ] ]'
...
```

#### <a name="apidoc.element.natural.NGrams.setTokenizer"></a>[function <span class="apidocSignatureSpan">natural.NGrams.</span>setTokenizer (t)](#apidoc.element.natural.NGrams.setTokenizer)
- description and source-code
```javascript
setTokenizer = function (t) {
    if(!_.isFunction(t.tokenize))
        throw new Error('Expected a valid Tokenizer');
    tokenizer = t;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NGrams.trigrams"></a>[function <span class="apidocSignatureSpan">natural.NGrams.</span>trigrams (sequence, startSymbol, endSymbol)](#apidoc.element.natural.NGrams.trigrams)
- description and source-code
```javascript
trigrams = function (sequence, startSymbol, endSymbol) {
    return ngrams(sequence, 3, startSymbol, endSymbol);
}
```
- example usage
```shell
...
'''

Both of the above output: '[ [ 'some', 'words' ], [ 'words', 'here' ] ]'

### trigrams

'''javascript
console.log(NGrams.trigrams('some other words here'));
console.log(NGrams.trigrams(['some',  'other', 'words',  'here']));
'''

Both of the above output: '[ [ 'some', 'other', 'words' ],
  [ 'other', 'words', 'here' ] ]'

### arbitrary n-grams
...
```



# <a name="apidoc.module.natural.NGramsZH"></a>[module natural.NGramsZH](#apidoc.module.natural.NGramsZH)

#### <a name="apidoc.element.natural.NGramsZH.bigrams"></a>[function <span class="apidocSignatureSpan">natural.NGramsZH.</span>bigrams (sequence, startSymbol, endSymbol)](#apidoc.element.natural.NGramsZH.bigrams)
- description and source-code
```javascript
bigrams = function (sequence, startSymbol, endSymbol) {
    return ngrams(sequence, 2, startSymbol, endSymbol);
}
```
- example usage
```shell
...
'''javascript
var NGrams = natural.NGrams;
'''

### bigrams

'''javascript
console.log(NGrams.bigrams('some words here'));
console.log(NGrams.bigrams(['some',  'words',  'here']));
'''

Both of the above output: '[ [ 'some', 'words' ], [ 'words', 'here' ] ]'

### trigrams
...
```

#### <a name="apidoc.element.natural.NGramsZH.ngrams"></a>[function <span class="apidocSignatureSpan">natural.NGramsZH.</span>ngrams (sequence, n, startSymbol, endSymbol)](#apidoc.element.natural.NGramsZH.ngrams)
- description and source-code
```javascript
ngrams = function (sequence, n, startSymbol, endSymbol) {
    return ngrams(sequence, n, startSymbol, endSymbol);
}
```
- example usage
```shell
...

Both of the above output: '[ [ 'some', 'other', 'words' ],
[ 'other', 'words', 'here' ] ]'

### arbitrary n-grams

'''javascript
console.log(NGrams.ngrams('some other words here for you', 4));
console.log(NGrams.ngrams(['some', 'other', 'words', 'here', 'for',
  'you'], 4));
'''

The above outputs: '[ [ 'some', 'other', 'words', 'here' ],
[ 'other', 'words', 'here', 'for' ],
[ 'words', 'here', 'for', 'you' ] ]'
...
```

#### <a name="apidoc.element.natural.NGramsZH.trigrams"></a>[function <span class="apidocSignatureSpan">natural.NGramsZH.</span>trigrams (sequence, startSymbol, endSymbol)](#apidoc.element.natural.NGramsZH.trigrams)
- description and source-code
```javascript
trigrams = function (sequence, startSymbol, endSymbol) {
    return ngrams(sequence, 3, startSymbol, endSymbol);
}
```
- example usage
```shell
...
'''

Both of the above output: '[ [ 'some', 'words' ], [ 'words', 'here' ] ]'

### trigrams

'''javascript
console.log(NGrams.trigrams('some other words here'));
console.log(NGrams.trigrams(['some',  'other', 'words',  'here']));
'''

Both of the above output: '[ [ 'some', 'other', 'words' ],
  [ 'other', 'words', 'here' ] ]'

### arbitrary n-grams
...
```



# <a name="apidoc.module.natural.NounInflector"></a>[module natural.NounInflector](#apidoc.module.natural.NounInflector)

#### <a name="apidoc.element.natural.NounInflector.NounInflector"></a>[function <span class="apidocSignatureSpan">natural.</span>NounInflector ()](#apidoc.element.natural.NounInflector.NounInflector)
- description and source-code
```javascript
NounInflector = function () {
    this.ambiguous = [
        'bison', 'bream', 'carp', 'chassis', 'cod', 'corps', 'debris', 'deer',
        'diabetes', 'equipment', 'elk', 'fish', 'flounder', 'gallows', 'graffiti',
        'headquarters', 'herpes', 'highjinks', 'homework', 'information',
        'mackerel', 'mews', 'money', 'news', 'rice', 'rabies', 'salmon', 'series',
        'sheep', 'shrimp', 'species', 'swine', 'trout', 'tuna', 'whiting', 'wildebeest'
    ];

    this.customPluralForms = [];
    this.customSingularForms = [];
    this.singularForms = new FormSet();
    this.pluralForms = new FormSet();

    this.attach = attach;

    this.addIrregular("child", "children");
    this.addIrregular("man", "men");
    this.addIrregular("person", "people");
    this.addIrregular("sex", "sexes");
    this.addIrregular("mouse", "mice");
    this.addIrregular("ox", "oxen");
    this.addIrregular("foot", "feet");
    this.addIrregular("tooth", "teeth");
    this.addIrregular("goose", "geese");
    this.addIrregular("ephemeris", "ephemerides");

    // see if it is possible to unify the creation of both the singular and
    // plural regexes or maybe even just have one list. with a complete list
    // of rules it may only be possible for some regular forms, but worth a shot
    this.pluralForms.regularForms.push([/y$/i, 'ies']);
    this.pluralForms.regularForms.push([/ife$/i, 'ives']);
    this.pluralForms.regularForms.push([/(antenn|formul|nebul|vertebr|vit)a$/i, '$1ae']);
    this.pluralForms.regularForms.push([/(octop|vir|radi|nucle|fung|cact|stimul)us$/i, '$1i']);
    this.pluralForms.regularForms.push([/(buffal|tomat|tornad)o$/i, '$1oes']);
    this.pluralForms.regularForms.push([/(sis)$/i, 'ses']);
    this.pluralForms.regularForms.push([/(matr|vert|ind|cort)(ix|ex)$/i, '$1ices']);
    this.pluralForms.regularForms.push([/sses$/i, 'sses']);
    this.pluralForms.regularForms.push([/(x|ch|ss|sh|s|z)$/i, '$1es']);
    this.pluralForms.regularForms.push([/^(?!talis|.*hu)(.*)man$/i, '$1men']);
    this.pluralForms.regularForms.push([/(.*)/i, '$1s']);

    this.singularForms.regularForms.push([/([^v])ies$/i, '$1y']);
    this.singularForms.regularForms.push([/ives$/i, 'ife']);
    this.singularForms.regularForms.push([/(antenn|formul|nebul|vertebr|vit)ae$/i, '$1a']);
    this.singularForms.regularForms.push([/(octop|vir|radi|nucle|fung|cact|stimul)(i)$/i, '$1us']);
    this.singularForms.regularForms.push([/(buffal|tomat|tornad)(oes)$/i, '$1o']);
    this.singularForms.regularForms.push([/(analy|naly|synop|parenthe|diagno|the)ses$/i, '$1sis']);
    this.singularForms.regularForms.push([/(vert|ind|cort)(ices)$/i, '$1ex']);
    // our pluralizer won''t cause this form of appendix (appendicies)
    // but we should handle it
    this.singularForms.regularForms.push([/(matr|append)(ices)$/i, '$1ix']);
    this.singularForms.regularForms.push([/(x|ch|ss|sh|s|z)es$/i, '$1']);
    this.singularForms.regularForms.push([/men$/i, 'man']);
    this.singularForms.regularForms.push([/ss$/i, 'ss']);
    this.singularForms.regularForms.push([/s$/i, '']);

    this.pluralize = function (token) {
        return this.ize(token, this.pluralForms, this.customPluralForms);
    };

    this.singularize = function(token) {
        return this.ize(token, this.singularForms, this.customSingularForms);
    };
}
```
- example usage
```shell
...

### Nouns

Nouns can be pluralized/singularized with a 'NounInflector':

'''javascript
var natural = require('natural'),
nounInflector = new natural.NounInflector();
'''

To pluralize a word (outputs "radii"):

'''javascript
console.log(nounInflector.pluralize('radius'));
'''
...
```

#### <a name="apidoc.element.natural.NounInflector.super_"></a>[function <span class="apidocSignatureSpan">natural.NounInflector.</span>super_ ()](#apidoc.element.natural.NounInflector.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.NounInflector.super_"></a>[module natural.NounInflector.super_](#apidoc.module.natural.NounInflector.super_)

#### <a name="apidoc.element.natural.NounInflector.super_.super_"></a>[function <span class="apidocSignatureSpan">natural.NounInflector.</span>super_ ()](#apidoc.element.natural.NounInflector.super_.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.NounInflector.super_.prototype"></a>[module natural.NounInflector.super_.prototype](#apidoc.module.natural.NounInflector.super_.prototype)

#### <a name="apidoc.element.natural.NounInflector.super_.prototype.addForm"></a>[function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>addForm (singularTable, pluralTable, singular, plural)](#apidoc.element.natural.NounInflector.super_.prototype.addForm)
- description and source-code
```javascript
addForm = function (singularTable, pluralTable, singular, plural) {
    singular = singular.toLowerCase();
    plural = plural.toLowerCase();
    pluralTable[singular] = plural;
    singularTable[plural] = singular;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NounInflector.super_.prototype.addIrregular"></a>[function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>addIrregular (singular, plural)](#apidoc.element.natural.NounInflector.super_.prototype.addIrregular)
- description and source-code
```javascript
addIrregular = function (singular, plural) {
    this.addForm(this.singularForms.irregularForms, this.pluralForms.irregularForms, singular, plural);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NounInflector.super_.prototype.addPlural"></a>[function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>addPlural (pattern, replacement)](#apidoc.element.natural.NounInflector.super_.prototype.addPlural)
- description and source-code
```javascript
addPlural = function (pattern, replacement) {
    this.customPluralForms.push([pattern, replacement]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NounInflector.super_.prototype.addSingular"></a>[function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>addSingular (pattern, replacement)](#apidoc.element.natural.NounInflector.super_.prototype.addSingular)
- description and source-code
```javascript
addSingular = function (pattern, replacement) {
    this.customSingularForms.push([pattern, replacement]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NounInflector.super_.prototype.ize"></a>[function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>ize (token, formSet, customForms)](#apidoc.element.natural.NounInflector.super_.prototype.ize)
- description and source-code
```javascript
ize = function (token, formSet, customForms) {
    var restoreCase = this.restoreCase(token);
    return restoreCase(this.izeRegExps(token, customForms) || this.izeAbiguous(token) ||
        this.izeRegulars(token, formSet) || this.izeRegExps(token, formSet.regularForms) ||
        token);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NounInflector.super_.prototype.izeAbiguous"></a>[function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>izeAbiguous (token)](#apidoc.element.natural.NounInflector.super_.prototype.izeAbiguous)
- description and source-code
```javascript
izeAbiguous = function (token) {
    if(this.ambiguous.indexOf(token.toLowerCase()) > -1)
        return token.toLowerCase();

    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NounInflector.super_.prototype.izeRegExps"></a>[function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>izeRegExps (token, forms)](#apidoc.element.natural.NounInflector.super_.prototype.izeRegExps)
- description and source-code
```javascript
izeRegExps = function (token, forms) {
    var i, form;
    for(i = 0; i < forms.length; i++) {
        form = forms[i];

        if(token.match(form[0]))
            return token.replace(form[0], form[1]);
    }

    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NounInflector.super_.prototype.izeRegulars"></a>[function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>izeRegulars (token, formSet)](#apidoc.element.natural.NounInflector.super_.prototype.izeRegulars)
- description and source-code
```javascript
izeRegulars = function (token, formSet) {
    token = token.toLowerCase();
    if(formSet.irregularForms.hasOwnProperty(token) && formSet.irregularForms[token])
        return formSet.irregularForms[token];

    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NounInflector.super_.prototype.pluralize"></a>[function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>pluralize (token)](#apidoc.element.natural.NounInflector.super_.prototype.pluralize)
- description and source-code
```javascript
pluralize = function (token) {
    return this.ize(token, this.pluralForms, this.customPluralForms);
}
```
- example usage
```shell
...
var natural = require('natural'),
nounInflector = new natural.NounInflector();
'''

To pluralize a word (outputs "radii"):

'''javascript
console.log(nounInflector.pluralize('radius'));
'''

To singularize a word (outputs "beer"):

'''javascript
console.log(nounInflector.singularize('beers'));
'''
...
```

#### <a name="apidoc.element.natural.NounInflector.super_.prototype.restoreCase"></a>[function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>restoreCase (token)](#apidoc.element.natural.NounInflector.super_.prototype.restoreCase)
- description and source-code
```javascript
restoreCase = function (token) {
    if (token[0] === token[0].toUpperCase()) {
        if (token[1] && token[1] === token[1].toLowerCase()) {
            return capitalize;
        } else {
            return uppercaseify;
        }
    } else {
        return lowercaseify;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NounInflector.super_.prototype.singularize"></a>[function <span class="apidocSignatureSpan">natural.NounInflector.super_.prototype.</span>singularize (token)](#apidoc.element.natural.NounInflector.super_.prototype.singularize)
- description and source-code
```javascript
singularize = function (token) {
    return this.ize(token, this.singularForms, this.customSingularForms);
}
```
- example usage
```shell
...
'''javascript
console.log(nounInflector.pluralize('radius'));
'''

To singularize a word (outputs "beer"):

'''javascript
console.log(nounInflector.singularize('beers'));
'''

Like many of the other features, String can be patched to perform the operations
directly. The "Noun" suffix on the methods is necessary, as verbs will be
supported in the future.

'''javascript
...
```



# <a name="apidoc.module.natural.NounInflectorFr"></a>[module natural.NounInflectorFr](#apidoc.module.natural.NounInflectorFr)

#### <a name="apidoc.element.natural.NounInflectorFr.NounInflectorFr"></a>[function <span class="apidocSignatureSpan">natural.</span>NounInflectorFr ()](#apidoc.element.natural.NounInflectorFr.NounInflectorFr)
- description and source-code
```javascript
NounInflectorFr = function () {
  // Ambiguous a.k.a. invariant.
  // \@todo Expand this list to be as comprehensive as possible.
  this.ambiguous = [
    // Nouns ending by -s
    'à-peu-près', 'à-propos', 'abattis', 'abcès', 'abois', 'abribus', 'abus',
    'accès', 'acquis', 'adénovirus', 'adonis', 'ados', 'agrès', 'aguets',
    'ailleurs', 'ais', 'albatros', 'albinos', 'alias', 'aloès', 'amaryllis',
    'amas', 'ampélopsis', 'ananas', 'anchois', 'angélus', 'anis', 'anticorps',
    'antihéros', 'antirides', 'anus', 'appas', 'appentis', 'appui-bras',
    'appuie-bras', 'arcanes', 'argus', 'arrérages', 'arrière-pays', 'as',
    'ascaris', 'asparagus', 'atlas', 'atours', 'aurochs', 'autobus',
    'autofocus', 'avant-bras', 'avant-corps', 'avant-propos', 'avers', 'avis',
    'axis', 'barbouillis', 'bas', 'beaujolais', 'beaux-arts', 'biais',
    'bibliobus', 'biceps', 'bicross', 'bien-fonds', 'bloc-notes', 'blockhaus',
    'blocus', 'blues', 'bois', 'bonus', 'bout-dehors', 'bouts-rimés',
    'branle-bas', 'bras', 'brebis', 'bris', 'brise-lames', 'brise-mottes',
    'brûlis', 'buis', 'burnous', 'bus', 'business', 'cabas', 'cacatoès',
    'cacatois', 'cactus', 'cadenas', 'cafouillis', 'caillebotis', 'calvados',
    'cambouis', 'campus', 'canevas', 'cannabis', 'carquois', 'cas',
    'casse-noisettes', 'casse-pieds', 'cassis', 'caucus', 'cens', 'cervelas',
    'chablis', 'chamois', 'chaos', 'chas', 'chasselas', 'châssis',
    'chatouillis', 'chauffe-assiettes', 'chauve-souris', 'chorus', 'choucas',
    'circoncis', 'cirrus', 'clafoutis', 'clapotis', 'cliquetis', 'clos',
    'cochylis', 'colis', 'coloris', 'commis', 'compas', 'compromis',
    'compte-chèques', 'compte-gouttes', 'compte-tours', 'concours', 'confins',
    'congrès', 'consensus', 'contrepoids', 'contresens', 'contretemps',
    'corn flakes', 'corps', 'corps-à-corps', 'corpus', 'cosinus', 'cosmos',
    'coulis', 'coupe-ongles', 'cours', 'court-jus', 'couscous', 'coutelas',
    'crocus', 'croquis', 'cross', 'cubitus', 'cumulus', 'cure-dents',
    'cure-ongles', 'cure-pipes', 'cursus', 'cyclo-cross', 'cyprès', 'dais',
    'damas', 'débarras', 'débours', 'débris', 'décès', 'dedans', 'dehors',
    'delirium tremens', 'demi-gros', 'dépens', 'dessous', 'dessus', 'détritus',
    'deux-mâts', 'deux-pièces', 'deux-points', 'deux-roues', 'deux-temps',
    'dévers', 'devis', 'diplodocus', 'discours', 'dos', 'ébats', 'éboulis',
    'échalas', 'edelweiss', 'élaeis', 'éleis', 'éléphantiasis', 'embarras',
    'empois', 'en-cas', 'encens', 'enclos', 'endos', 'engrais', 'entrelacs',
    'entremets', 'envers', 'épluche-légumes', 'ers', 'espace-temps',
    'essuie-mains', 'eucalyptus', 'ex-libris', 'excès', 'express', 'extrados',
    'faciès', 'fait-divers', 'fatras', 'faux-sens', 'favoris', 'ficus',
    'fier-à-bras', 'finnois', 'florès', 'focus', 'fœtus', 'fois', 'forceps',
    'fouillis', 'fracas', 'frais', 'français', 'franglais', 'frimas',
    'friselis', 'frisottis', 'froncis', 'frottis', 'fucus', 'gâchis', 'galetas',
    'galimatias', 'garde-à-vous', 'garde-corps', 'gargouillis', 'gars',
    'gâte-bois', 'gazouillis', 'génois', 'gibus', 'glacis', 'glas', 'gneiss',
    'gobe-mouches', 'grès', 'gribouillis', 'guet-apens', 'habeas corpus',
    'hachis', 'haras', 'hardes', 'harnais', 'haut-le-corps', 'hautbois',
    'herbe-aux-chats', 'héros', 'herpès', 'hiatus', 'hibiscus', 'hors-concours',
    'hors-pistes', 'hourdis', 'huis-clos', 'humérus', 'humus', 'ibis', 'iléus',
    'indique-fuites', 'infarctus', 'inlandsis', 'insuccès', 'intercours',
    'intrados', 'intrus', 'iris', 'isatis', 'jais', 'jars', 'jeans',
    'jeuconcours', 'judas', 'juliénas', 'jus', 'justaucorps', 'kakatoès',
    'kermès', 'kriss', 'lacis', 'laïus', 'lambris', 'lapis', 'laps', 'lapsus',
    'laquais', 'las', 'lattis', 'lave-mains', 'lavis', 'lèche-bottes',
    'lèche-vitrines', 'legs', 'lias', 'liégeois', 'lilas', 'lis', 'lœss',
    'logis', 'loris', 'lotus', 'louis', 'lupus', 'lys', 'mâchicoulis', 'madras',
    'maïs', 'malappris', 'malus', 'mânes', 'maquis', 'marais', 'maroilles',
    'marquis', 'mas', 'mass-médias', 'matel ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NounInflectorFr.super_"></a>[function <span class="apidocSignatureSpan">natural.NounInflectorFr.</span>super_ ()](#apidoc.element.natural.NounInflectorFr.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.NounInflectorJa"></a>[module natural.NounInflectorJa](#apidoc.module.natural.NounInflectorJa)

#### <a name="apidoc.element.natural.NounInflectorJa.NounInflectorJa"></a>[function <span class="apidocSignatureSpan">natural.</span>NounInflectorJa ()](#apidoc.element.natural.NounInflectorJa.NounInflectorJa)
- description and source-code
```javascript
NounInflectorJa = function () {
  // Ambiguous a.k.a. invariant.
  this.ambiguous = [
    'ともだち', '友だち', '友達', '遊び友達', '飲み友達', '酒飲み友達', '茶飲み友達',
    '学校友達', '女友達', '男友達', '幼友達'
  ];

  this.customPluralForms = [];
  this.customSingularForms = [];
  this.singularForms = new FormSet();
  this.pluralForms = new FormSet();

  this.attach = attach;

  this.addIrregular('神', '神神');
  this.addIrregular('人', '人人');
  this.addIrregular('年', '年年');
  this.addIrregular('月', '月月');
  this.addIrregular('日', '日日');
  this.addIrregular('星', '星星');
  this.addIrregular('島', '島島');
  this.addIrregular('我', '我我');
  this.addIrregular('山', '山山');
  this.addIrregular('国', '国国');
  this.addIrregular('所', '所所');
  this.addIrregular('隅', '隅隅');

<span class="apidocCodeCommentSpan">  /**
   * Notes:
   * -たち exceptions: いたち, おいたち, ついたち, かたち, かおかたち, なりかたち, いでたち, はたち, からたち, なりたち
   * -達 exceptions: 伊達, 男伊達, 栄達, 上意下達, 熟達, 上達, 下意上達, 先達, 送達, 速達, 即日速達, 書留速達, 調達, 通達, 伝達, 到達, 配達, 牛乳配達, 新聞配達, 無料配達, 四通八達, 発達, 未発達, 御用達, 宮内庁御用達, 練達, 闊達
   * -等 exceptions: 一等, 下等, 何等, 均等, 勲等, 高等, 三等, 初等, 上等, 親等, 二親等, 数等, 対等, 中等, 同等, 特等, 二等, 品等, 不等, 平等, 悪平等, 男女平等, 不平等, 優等, 劣等
   */
</span>
  // Pluralize
  this.pluralForms.regularForms.push([/^(.+)$/i, '$1たち']);

  // Singularize
  this.singularForms.regularForms.push([/^(.+)たち$/i, function(a, mask) {
    if (['い', 'おい', 'つい', 'か', 'かおか', 'なりか', 'いで', 'は', 'から',
      'なり'].indexOf(mask) >= 0)
      return mask + 'たち';
    return mask;
  }]);
  this.singularForms.regularForms.push([/^(.+)達$/i, function(a, mask) {
    if (['伊', '伊', '栄', '上意下', '熟', '上', '下意上', '先', '送', '速',
      '即日速', '書留速', '調', '通', '伝', '到', '配', '牛乳配', '新聞配', '無料配',
      '四通八', '発', '未発', '御用', '宮内庁御用', '練', '闊'].indexOf(mask) >= 0)
      return mask + '達';
    return mask;
  }]);  // Singularize nouns ending by -等, but not exceptions.
  this.singularForms.regularForms.push([/^(.+)等$/i, function(a, mask) {
    if (['一', '下', '何', '均', '勲', '高', '三', '初', '親', '二親', '数', '対',
      '中', '同', '特', '二', '品', '不', '平', '悪平', '男女平', '不平', '優',
      '劣'].indexOf(mask) >= 0)
      return mask + '等';
    return mask;
  }]);
  this.singularForms.regularForms.push([/^(人間|わたくし|私|てまえ|手前|野郎|やろう|勇者|がき|ガキ|餓鬼|あくとう|悪党|猫|家来)(共|ども)$/i, '$1']);
  this.singularForms.regularForms.push([/^(神様|先生|あなた|大名|女中|奥様)(方|がた)$/i, '$1']);

  this.pluralize = function(token) {
    return this.ize(token, this.pluralForms, this.customPluralForms);
  };

  this.singularize = function(token) {
    return this.ize(token, this.singularForms, this.customSingularForms);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.NounInflectorJa.super_"></a>[function <span class="apidocSignatureSpan">natural.NounInflectorJa.</span>super_ ()](#apidoc.element.natural.NounInflectorJa.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.PorterStemmer"></a>[module natural.PorterStemmer](#apidoc.module.natural.PorterStemmer)

#### <a name="apidoc.element.natural.PorterStemmer.addStopWord"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>addStopWord (stopWord)](#apidoc.element.natural.PorterStemmer.addStopWord)
- description and source-code
```javascript
addStopWord = function (stopWord) {
    stopwords.words.push(stopWord);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmer.addStopWords"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>addStopWords (moreStopWords)](#apidoc.element.natural.PorterStemmer.addStopWords)
- description and source-code
```javascript
addStopWords = function (moreStopWords) {
    stopwords.words = stopwords.words.concat(moreStopWords);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmer.attach"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>attach ()](#apidoc.element.natural.PorterStemmer.attach)
- description and source-code
```javascript
attach = function () {
    String.prototype.stem = function() {
        return stemmer.stem(this);
    };

    String.prototype.tokenizeAndStem = function(keepStops) {
        return stemmer.tokenizeAndStem(this, keepStops);
    };
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.PorterStemmer.categorizeGroups"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>categorizeGroups (token)](#apidoc.element.natural.PorterStemmer.categorizeGroups)
- description and source-code
```javascript
function categorizeGroups(token) {
    return token.replace(/[^aeiouy]+y/g, 'CV').replace(/[aeiou]+/g, 'V').replace(/[^V]+/g, 'C');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmer.measure"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>measure (token)](#apidoc.element.natural.PorterStemmer.measure)
- description and source-code
```javascript
function measure(token) {
    if(!token)
    	return -1;

    return categorizeGroups(token).replace(/^C/, '').replace(/V$/, '').length / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmer.removeStopWord"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>removeStopWord (stopWord)](#apidoc.element.natural.PorterStemmer.removeStopWord)
- description and source-code
```javascript
removeStopWord = function (stopWord) {
    this.removeStopWords([stopWord])
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmer.removeStopWords"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>removeStopWords (moreStopWords)](#apidoc.element.natural.PorterStemmer.removeStopWords)
- description and source-code
```javascript
removeStopWords = function (moreStopWords) {
    moreStopWords.forEach(function(stopWord){
        var idx = stopwords.words.indexOf(stopWord);
        if (idx >= 0) {
            stopwords.words.splice(idx, 1);
        }
    });

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmer.stem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>stem (token)](#apidoc.element.natural.PorterStemmer.stem)
- description and source-code
```javascript
stem = function (token) {
    if(token.length < 3) return token;
    return step5b(step5a(step4(step3(step2(step1c(step1b(step1a(token.toLowerCase())))))))).toString();
}
```
- example usage
```shell
...
'''javascript
var natural = require('natural');
'''

This example uses a Porter stemmer. "word" is returned.

'''javascript
console.log(natural.PorterStemmer.stem("words")); // stem a single word
'''

 in Russian:

'''javascript
console.log(natural.PorterStemmerRu.stem("падший"));
'''
...
```

#### <a name="apidoc.element.natural.PorterStemmer.step1a"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step1a (token)](#apidoc.element.natural.PorterStemmer.step1a)
- description and source-code
```javascript
function step1a(token) {
    if(token.match(/(ss|i)es$/)) {
        return token.replace(/(ss|i)es$/, '$1');
    }

    if(token.substr(-1) == 's' && token.substr(-2, 1) != 's' && token.length > 2) {
        return token.replace(/s?$/, '');
    }

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmer.step1b"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step1b (token)](#apidoc.element.natural.PorterStemmer.step1b)
- description and source-code
```javascript
function step1b(token) {
    if(token.substr(-3) == 'eed') {
        if(measure(token.substr(0, token.length - 3)) > 0)
            return token.replace(/eed$/, 'ee');
    } else {
        var result = attemptReplace(token, /(ed|ing)$/, '', function(token) {
            if(categorizeGroups(token).indexOf('V') >= 0) {
                result = attemptReplacePatterns(token, [['at', '', 'ate'],  ['bl', '', 'ble'], ['iz', '', 'ize']]);

                if(result != token) {
        		    return result;
        		} else {
        		  if(endsWithDoublCons(token) && token.match(/[^lsz]$/)) {
        			 return token.replace(/([^aeiou])\1$/, '$1');
                    }

        		  if(measure(token) == 1 && categorizeChars(token).substr(-3) == 'CVC' && token.match(/[^wxy]$/)) {
        			 return token + 'e';
                    }
        		}

        		return token;
    	    }
    	
    	    return null;
    	});
    	
    	if(result) {
    	    return result;
        }
    }

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmer.step1c"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step1c (token)](#apidoc.element.natural.PorterStemmer.step1c)
- description and source-code
```javascript
function step1c(token) {
    var categorizedGroups = categorizeGroups(token);

    if(token.substr(-1) == 'y' && categorizedGroups.substr(0, categorizedGroups.length - 1).indexOf('V') > -1) {
        return token.replace(/y$/, 'i');
    }

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmer.step2"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step2 (token)](#apidoc.element.natural.PorterStemmer.step2)
- description and source-code
```javascript
function step2(token) {
    token = replacePatterns(token, [['ational', '', 'ate'], ['tional', '', 'tion'], ['enci', '', 'ence'], ['anci', '', 'ance'],
        ['izer', '', 'ize'], ['abli', '', 'able'], ['bli', '', 'ble'], ['alli', '', 'al'], ['entli', '', 'ent'], ['eli', '', 'e'],
        ['ousli', '', 'ous'], ['ization', '', 'ize'], ['ation', '', 'ate'], ['ator', '', 'ate'],['alism', '', 'al'],
        ['iveness', '', 'ive'], ['fulness', '', 'ful'], ['ousness', '', 'ous'], ['aliti', '', 'al'],
        ['iviti', '', 'ive'], ['biliti', '', 'ble'], ['logi', '', 'log']], 0);

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmer.step3"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step3 (token)](#apidoc.element.natural.PorterStemmer.step3)
- description and source-code
```javascript
function step3(token) {
    return replacePatterns(token, [['icate', '', 'ic'], ['ative', '', ''], ['alize', '', 'al'],
				   ['iciti', '', 'ic'], ['ical', '', 'ic'], ['ful', '', ''], ['ness', '', '']], 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmer.step4"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step4 (token)](#apidoc.element.natural.PorterStemmer.step4)
- description and source-code
```javascript
function step4(token) {
    return replaceRegex(token, /^(.+?)(al|ance|ence|er|ic|able|ible|ant|ement|ment|ent|ou|ism|ate|iti|ous|ive|ize)$/, [1], 1) ||
        replaceRegex(token, /^(.+?)(s|t)(ion)$/, [1, 2], 1) ||
        token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmer.step5a"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step5a (token)](#apidoc.element.natural.PorterStemmer.step5a)
- description and source-code
```javascript
function step5a(token) {
    var m = measure(token.replace(/e$/, ''));



    if(m > 1 || (m == 1 && !(categorizeChars(token).substr(-4, 3) == 'CVC' && token.match(/[^wxy].$/)))) {
        token = token.replace(/e$/, '');
    }

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmer.step5b"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>step5b (token)](#apidoc.element.natural.PorterStemmer.step5b)
- description and source-code
```javascript
function step5b(token) {
    if(measure(token) > 1) {
       return token.replace(/ll$/, 'l');
    }

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmer.tokenizeAndStem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmer.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmer.tokenizeAndStem)
- description and source-code
```javascript
tokenizeAndStem = function (text, keepStops) {
    var stemmedTokens = [];
    var lowercaseText = text.toLowerCase();
    var tokens = new Tokenizer().tokenize(lowercaseText);

    if (keepStops) {
        tokens.forEach(function(token) {
            stemmedTokens.push(stemmer.stem(token));
        });
    }

    else {
        tokens.forEach(function(token) {
            if (stopwords.words.indexOf(token) == -1)
                stemmedTokens.push(stemmer.stem(token));
        });
    }

    return stemmedTokens;
}
```
- example usage
```shell
...

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
natural.LancasterStemmer.attach();
...
```



# <a name="apidoc.module.natural.PorterStemmerEs"></a>[module natural.PorterStemmerEs](#apidoc.module.natural.PorterStemmerEs)

#### <a name="apidoc.element.natural.PorterStemmerEs.attach"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerEs.</span>attach ()](#apidoc.element.natural.PorterStemmerEs.attach)
- description and source-code
```javascript
attach = function () {
    String.prototype.stem = function() {
        return stemmer.stem(this);
    };

    String.prototype.tokenizeAndStem = function(keepStops) {
        return stemmer.tokenizeAndStem(this, keepStops);
    };
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.PorterStemmerEs.stem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerEs.</span>stem (token)](#apidoc.element.natural.PorterStemmerEs.stem)
- description and source-code
```javascript
stem = function (token) {
	token = token.toLowerCase();

	if (token.length<3){
		return token;
	}

	var r1,r2,rv,len= token.length;
	//looking for regions after vowels

	for(var i=0; i< token.length-1 && r1==len;i++){
 		if(isVowel(token[i]) && !isVowel(token[i+1]) ){
 			r1=i+2;
 		}

	}

	for(var i=r1; i< token.length-1 && r2==len;i++){
		if(isVowel(token[i]) && !isVowel(token[i+1])){
			r2=i+2;
		}
	}

	if (len > 3) {
			if(isVowel(token[1])) {
				// If the second letter is a consonant, RV is the region after the next following vowel
				rv = getNextVowelPos(token, 2) +1;
			} else if (isVowel(token[0]) && isVowel(token[1])) {
				// or if the first two letters are vowels, RV is the region after the next consonant
				rv = getNextConsonantPos(token, 2) + 1;
			} else {
				//otherwise (consonant-vowel case) RV is the region after the third letter. But RV is the end of the word if these positions
 cannot be found.
				rv = 3;
			}
		}

	var r1_txt = token.substring(r1-1);
	var r2_txt = token.substring(r2-1);
	var rv_txt = token.substring(rv-1);


	var token_orig = token;

	// Step 0: Attached pronoun
	var pronoun_suf = new Array('me', 'se', 'sela', 'selo', 'selas', 'selos', 'la', 'le', 'lo', 'las', 'les', 'los', 'nos');
	var pronoun_suf_pre1 = new Array('éndo', 'ándo', 'ár', 'ér', 'ír');
	var pronoun_suf_pre2 = new Array('ando', 'iendo', 'ar', 'er', 'ir');
	var suf = endsinArr(token, pronoun_suf);


	if (suf!='') {

		var pre_suff = endsinArr(rv_txt.slice(0,-suf.length),pronoun_suf_pre1);

		if (pre_suff != '') {

				token = removeAccent(token.slice(0,-suf.length));
		} else {
			var pre_suff = endsinArr(rv_txt.slice(0,-suf.length),pronoun_suf_pre2);

			if (pre_suff != '' ||
				(endsin(token, 'yendo' ) &&
				(token.slice(-suf.length-6,1) == 'u'))) {
				token = token.slice(0,-suf.length);
			}
		}
	}

		if (token != token_orig) {
			r1_txt = token.substring(r1-1);
			r2_txt = token.substring(r2-1);
			rv_txt = token.substring(rv-1);
		}
		var token_after0 = token;

		if ((suf = endsinArr(r2_txt, new Array('anza', 'anzas', 'ico', 'ica', 'icos', 'icas', 'ismo', 'ismos', 'able', 'ables', 'ible', '
ibles', 'ista', 'istas', 'oso', 'osa', 'osos', 'osas', 'amiento', 'amientos', 'imiento', 'imientos'))) != '') {
			token = token.slice(0, -suf.length);
		} else if ((suf = endsinArr(r2_txt, new  Array('icadora', 'icador', 'icación', 'icadoras', 'icadores', 'icaciones', 'icante', '
icantes', 'icancia', 'icancias', 'adora', 'ador', 'ación', 'adoras', 'adores', 'aciones', 'ante', 'antes', 'ancia', 'ancias'))) != '') {
			token = token.slice(0,  -suf.length);
		} else if ((suf = endsinArr(r2_txt, new  Array('logía', 'logías'))) != '') {
			token = token.slice(0,  -suf.length)+ 'log';
		} else if ((suf =endsinArr(r2_txt, new  Array('ución', 'uciones'))) != '') {
			token = token.slice(0,  -suf.length) + 'u';
		} else if ((suf = endsinArr(r2_txt, new  Array('encia', 'encias'))) != '') {
			token = token.slice(0,  -suf.length)+ 'ente';
		} else if ((suf = endsinArr(r2_txt, new  Array('ativamente', 'ivamente', 'osamente', 'icamente', 'adamente'))) != '') {
			token = token.slice(0,  -suf.length);
		} else if ((suf = endsinArr(r1_txt, new  Array('amente'))) != '') {
			token = token.slice(0,  -suf.length);
		} else if ((suf = endsinArr(r2_txt, new  Array('antemente', 'ablemente', 'iblemente', 'mente'))) != '') {
			token = token.slice(0,  -suf.length);
		} else if ((suf = endsinArr(r2_txt, new  Array('abilidad', 'abilidades', 'icidad', 'icidades', 'ividad', 'ividades', 'idad', '
idades'))) != '') {
			token = token.slice(0,  -suf.length);
		} else if ((suf = endsinArr(r2_txt, new  Array('ativa', 'ativo', 'ativas', 'ativos', 'iva', 'ivo', 'ivas', 'ivos'))) != '') {
			token = token.slice(0,  -suf.length);
		}

		if (token != token_after0) {
			r1_txt = token.substring(r1-1);
			r2_txt = token.substring(r2-1);
			rv_txt = token.substring(rv-1);
		}
		var token_after1 = token;

		if (token_after0 == token_after1) {
			// Do step 2a if no ending was removed by step 1.
			if ((suf = endsinArr(rv_txt, new Array('ya', 'ye', 'yan', 'yen', 'yeron', ...
```
- example usage
```shell
...
'''javascript
var natural = require('natural');
'''

This example uses a Porter stemmer. "word" is returned.

'''javascript
console.log(natural.PorterStemmer.stem("words")); // stem a single word
'''

 in Russian:

'''javascript
console.log(natural.PorterStemmerRu.stem("падший"));
'''
...
```

#### <a name="apidoc.element.natural.PorterStemmerEs.tokenizeAndStem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerEs.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmerEs.tokenizeAndStem)
- description and source-code
```javascript
tokenizeAndStem = function (text, keepStops) {
    var stemmedTokens = [];

    new Tokenizer().tokenize(text).forEach(function(token) {
        if (keepStops || stopwords.words.indexOf(token) == -1) {
            var resultToken = token.toLowerCase();
            if (resultToken.match(new RegExp('[a-záéíóúüñ0-9]+', 'gi'))) {
                resultToken = stemmer.stem(resultToken);
            }
            stemmedTokens.push(resultToken);
        }
    });

    return stemmedTokens;
}
```
- example usage
```shell
...

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
natural.LancasterStemmer.attach();
...
```



# <a name="apidoc.module.natural.PorterStemmerFa"></a>[module natural.PorterStemmerFa](#apidoc.module.natural.PorterStemmerFa)

#### <a name="apidoc.element.natural.PorterStemmerFa.attach"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerFa.</span>attach ()](#apidoc.element.natural.PorterStemmerFa.attach)
- description and source-code
```javascript
attach = function () {
    String.prototype.stem = function() {
        return stemmer.stem(this);
    };

    String.prototype.tokenizeAndStem = function(keepStops) {
        return stemmer.tokenizeAndStem(this, keepStops);
    };
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.PorterStemmerFa.stem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerFa.</span>stem (token)](#apidoc.element.natural.PorterStemmerFa.stem)
- description and source-code
```javascript
stem = function (token) {
    return token;
}
```
- example usage
```shell
...
'''javascript
var natural = require('natural');
'''

This example uses a Porter stemmer. "word" is returned.

'''javascript
console.log(natural.PorterStemmer.stem("words")); // stem a single word
'''

 in Russian:

'''javascript
console.log(natural.PorterStemmerRu.stem("падший"));
'''
...
```

#### <a name="apidoc.element.natural.PorterStemmerFa.tokenizeAndStem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerFa.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmerFa.tokenizeAndStem)
- description and source-code
```javascript
tokenizeAndStem = function (text, keepStops) {
    var stemmedTokens = [];

    new Tokenizer().tokenize(text).forEach(function(token) {
        if(keepStops || stopwords.words.indexOf(token) == -1)
            stemmedTokens.push(stemmer.stem(token));
    });

    return stemmedTokens;
}
```
- example usage
```shell
...

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
natural.LancasterStemmer.attach();
...
```



# <a name="apidoc.module.natural.PorterStemmerFr"></a>[module natural.PorterStemmerFr](#apidoc.module.natural.PorterStemmerFr)

#### <a name="apidoc.element.natural.PorterStemmerFr.attach"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerFr.</span>attach ()](#apidoc.element.natural.PorterStemmerFr.attach)
- description and source-code
```javascript
attach = function () {
   String.prototype.stem = function() {
      return stemmer.stem(this);
   };

   String.prototype.tokenizeAndStem = function(keepStops) {
      return stemmer.tokenizeAndStem(this, keepStops);
   };
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.PorterStemmerFr.endsinArr"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerFr.</span>endsinArr (token, suffixes)](#apidoc.element.natural.PorterStemmerFr.endsinArr)
- description and source-code
```javascript
function endsinArr(token, suffixes) {
  var i, longest = '';
  for (i = 0; i < suffixes.length; i++) {
    if (endsin(token, suffixes[i]) && suffixes[i].length > longest.length)
      longest = suffixes[i];
  }

  return longest;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmerFr.prelude"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerFr.</span>prelude (token)](#apidoc.element.natural.PorterStemmerFr.prelude)
- description and source-code
```javascript
function prelude(token) {
  token = token.toLowerCase();

  var result = '';
  var i = 0;

  // special case for i = 0 to avoid '-1' index
  if (token[i] === 'y' && isVowel(token[i + 1])) {
    result += token[i].toUpperCase();
  } else {
    result += token[i];
  }

  for (i = 1; i < token.length; i++) {
    if ((token[i] === 'u' || token[i] === 'i') && isVowel(token[i - 1]) && isVowel(token[i + 1])) {
      result += token[i].toUpperCase();
    } else if (token[i] === 'y' && (isVowel(token[i - 1]) || isVowel(token[i + 1]))) {
      result += token[i].toUpperCase();
    } else if (token[i] === 'u' && token[i - 1] === 'q') {
      result += token[i].toUpperCase();
    } else {
      result += token[i];
    }
  }

  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmerFr.regions"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerFr.</span>regions (token)](#apidoc.element.natural.PorterStemmerFr.regions)
- description and source-code
```javascript
function regions(token) {
  var r1, r2, rv, len;
  var i;

  r1 = r2 = rv = len = token.length;

  // R1 is the region after the first non-vowel following a vowel,
  for (var i = 0; i < len - 1 && r1 == len; i++) {
    if (isVowel(token[i]) && !isVowel(token[i + 1])) {
      r1 = i + 2;
    }
  }
  // Or is the null region at the end of the word if there is no such non-vowel.

  // R2 is the region after the first non-vowel following a vowel in R1
  for (i = r1; i < len - 1 && r2 == len; i++) {
    if (isVowel(token[i]) && !isVowel(token[i + 1])) {
      r2 = i + 2;
    }
  }
  // Or is the null region at the end of the word if there is no such non-vowel.

  // RV region
  var three = token.slice(0, 3);
  if (isVowel(token[0]) && isVowel(token[1])) {
    rv = 3;
  }
  if (three === 'par' || three == 'col' || three === 'tap')
    rv = 3;
  // the region after the first vowel not at the beginning of the word or null
  else {
    for (i = 1; i < len - 1 && rv == len; i++) {
      if (isVowel(token[i])) {
        rv = i + 1;
      }
    }
  }

  return {
    r1: r1,
    r2: r2,
    rv: rv
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmerFr.stem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerFr.</span>stem (token)](#apidoc.element.natural.PorterStemmerFr.stem)
- description and source-code
```javascript
function stem(token) {
  token = prelude(token.toLowerCase());

  if (token.length == 1)
    return token;

  var regs = regions(token);

  var r1_txt, r2_txt, rv_txt;
  r1_txt = token.substring(regs.r1);
  r2_txt = token.substring(regs.r2);
  rv_txt = token.substring(regs.rv);

  // Step 1
  var beforeStep1 = token;
  var suf, pref2, pref3, letterBefore, letter2Before, i;
  var doStep2a = false;

  if ((suf = endsinArr(r2_txt, ['ance', 'iqUe', 'isme', 'able', 'iste', 'eux', 'ances', 'iqUes', 'ismes', 'ables', 'istes'])) != '') {
    token = token.slice(0, -suf.length); // delete
  } else if ((suf = endsinArr(token, ['icatrice', 'icateur', 'ication', 'icatrices', 'icateurs', 'ications'])) != '') {
    if (endsinArr(r2_txt, ['icatrice', 'icateur', 'ication', 'icatrices', 'icateurs', 'ications']) != '') {
      token = token.slice(0, -suf.length); // delete
    } else {
      token = token.slice(0, -suf.length) + 'iqU'; // replace by iqU
    }
  } else if ((suf = endsinArr(r2_txt, ['atrice', 'ateur', 'ation', 'atrices', 'ateurs', 'ations'])) != '') {
    token = token.slice(0, -suf.length); // delete
  } else if ((suf = endsinArr(r2_txt, ['logie', 'logies'])) != '') {
    token = token.slice(0, -suf.length) + 'log'; // replace with log
  } else if ((suf = endsinArr(r2_txt, ['usion', 'ution', 'usions', 'utions'])) != '') {
    token = token.slice(0, -suf.length) + 'u'; // replace with u
  } else if ((suf = endsinArr(r2_txt, ['ence', 'ences'])) != '') {
    token = token.slice(0, -suf.length) + 'ent'; // replace with ent
  }
  // ement(s)
  else if ((suf = endsinArr(r1_txt, ['issement', 'issements'])) != '') {
    if (!isVowel(token[token.length - suf.length - 1])) {
      token = token.slice(0, -suf.length); // delete
      r1_txt = token.substring(regs.r1);
      r2_txt = token.substring(regs.r2);
      rv_txt = token.substring(regs.rv);
    }
  } else if ((suf = endsinArr(r2_txt, ['ativement', 'ativements'])) != '') {
    token = token.slice(0, -suf.length); // delete
  } else if ((suf = endsinArr(r2_txt, ['ivement', 'ivements'])) != '') {
    token = token.slice(0, -suf.length); // delete
  } else if ((suf = endsinArr(token, ['eusement', 'eusements'])) != '') {
    if ((suf = endsinArr(r2_txt, ['eusement', 'eusements'])) != '')
      token = token.slice(0, -suf.length); // delete
    else if ((suf = endsinArr(r1_txt, ['eusement', 'eusements'])) != '')
      token = token.slice(0, -suf.length) + 'eux'; // replace by eux
    else if ((suf = endsinArr(rv_txt, ['ement', 'ements'])) != '')
      token = token.slice(0, -suf.length); // delete
  } else if ((suf = endsinArr(r2_txt, ['ablement', 'ablements', 'iqUement', 'iqUements'])) != '') {
    token = token.slice(0, -suf.length); // delete
  } else if ((suf = endsinArr(rv_txt, ['ièrement', 'ièrements', 'Ièrement', 'Ièrements'])) != '') {
    token = token.slice(0, -suf.length) + 'i'; // replace by i
  } else if ((suf = endsinArr(rv_txt, ['ement', 'ements'])) != '') {
    token = token.slice(0, -suf.length); // delete
  }
  // ité(s)
  else if ((suf = endsinArr(token, ['icité', 'icités'])) != '') {
    if (endsinArr(r2_txt, ['icité', 'icités']) != '')
      token = token.slice(0, -suf.length); // delete
    else
      token = token.slice(0, -suf.length) + 'iqU'; // replace by iqU
  } else if ((suf = endsinArr(token, ['abilité', 'abilités'])) != '') {
    if (endsinArr(r2_txt, ['abilité', 'abilités']) != '')
      token = token.slice(0, -suf.length); // delete
    else
      token = token.slice(0, -suf.length) + 'abl'; // replace by abl
  } else if ((suf = endsinArr(r2_txt, ['ité', 'ités'])) != '') {
    token = token.slice(0, -suf.length); // delete if in R2
  } else if ((suf = endsinArr(token, ['icatif', 'icative', 'icatifs', 'icatives'])) != '') {
    if ((suf = endsinArr(r2_txt, ['icatif', 'icative', 'icatifs', 'icatives'])) != '') {
      token = token.slice(0, -suf.length); // delete
      r2_txt = token.substring(regs.r2);
      rv_txt = token.substring(regs.rv);
    }
    if ((suf = endsinArr(r2_txt, ['atif', 'ative', 'atifs', 'atives'])) != '') {
      token = token.sl ...
```
- example usage
```shell
...
'''javascript
var natural = require('natural');
'''

This example uses a Porter stemmer. "word" is returned.

'''javascript
console.log(natural.PorterStemmer.stem("words")); // stem a single word
'''

 in Russian:

'''javascript
console.log(natural.PorterStemmerRu.stem("падший"));
'''
...
```

#### <a name="apidoc.element.natural.PorterStemmerFr.tokenizeAndStem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerFr.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmerFr.tokenizeAndStem)
- description and source-code
```javascript
tokenizeAndStem = function (text, keepStops) {
   var stemmedTokens = [];

   new Tokenizer().tokenize(text).forEach(function(token) {
      if (keepStops || stopwords.words.indexOf(token) == -1) {
         var resultToken = token.toLowerCase();
         if (resultToken.match(/[a-zâàëéêèïîôûùç0-9]/gi)) {
            resultToken = stemmer.stem(resultToken);
         }
         stemmedTokens.push(resultToken);
      }
   });

   return stemmedTokens;
}
```
- example usage
```shell
...

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
natural.LancasterStemmer.attach();
...
```



# <a name="apidoc.module.natural.PorterStemmerIt"></a>[module natural.PorterStemmerIt](#apidoc.module.natural.PorterStemmerIt)

#### <a name="apidoc.element.natural.PorterStemmerIt.attach"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerIt.</span>attach ()](#apidoc.element.natural.PorterStemmerIt.attach)
- description and source-code
```javascript
attach = function () {
    String.prototype.stem = function() {
        return stemmer.stem(this);
    };

    String.prototype.tokenizeAndStem = function(keepStops) {
        return stemmer.tokenizeAndStem(this, keepStops);
    };
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.PorterStemmerIt.stem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerIt.</span>stem (token)](#apidoc.element.natural.PorterStemmerIt.stem)
- description and source-code
```javascript
stem = function (token) {
	
	token = token.toLowerCase();
	token = replaceAcute(token);
	token = token.replace(/qu/g,'qU');	
	token = vowelMarking(token);
	
	if (token.length<3){
		return token;
	}

	var r1 = r2 = rv = len = token.length;
	// R1 is the region after the first non-vowel following a vowel,
	for(var i=0; i < token.length-1 && r1==len;i++){
 		if(isVowel(token[i]) && !isVowel(token[i+1]) ){
 			r1=i+2;
 		}
	}
	// Or is the null region at the end of the word if there is no such non-vowel.

	// R2 is the region after the first non-vowel following a vowel in R1
	for(var i=r1; i< token.length-1 && r2==len;i++){
		if(isVowel(token[i]) && !isVowel(token[i+1])){
			r2=i+2;
		}
	}

	// Or is the null region at the end of the word if there is no such non-vowel.

	// If the second letter is a consonant, RV is the region after the next following vowel,
	
	// RV as follow

	if (len > 3) {
		if(!isVowel(token[1])) {
			// If the second letter is a consonant, RV is the region after the next following vowel
			rv = getNextVowelPos(token, 1) +1;
		} else if (isVowel(token[0]) && isVowel(token[1])) {
			// or if the first two letters are vowels, RV is the region after the next consonant
			rv = getNextConsonantPos(token, 2) + 1;
		} else {
			//otherwise (consonant-vowel case) RV is the region after the third letter. But RV is the end of the word if these positions
cannot be found.
			rv = 3;
		}
	}

	var r1_txt = token.substring(r1);
	var r2_txt = token.substring(r2);
	var rv_txt = token.substring(rv);

	var token_orig = token;

	// Step 0: Attached pronoun

	var pronoun_suf = new Array('glieli','glielo','gliene','gliela','gliele','sene','tene','cela','cele','celi','celo','cene','vela
','vele','veli','velo','vene','mela','mele','meli','melo','mene','tela','tele','teli','telo','gli','ci', 'la','le','li','lo','mi
','ne','si','ti','vi');
	var pronoun_suf_pre1 = new Array('ando','endo');	
	var pronoun_suf_pre2 = new Array('ar', 'er', 'ir');
	var suf = endsinArr(token, pronoun_suf);

	if (suf!='') {
		var pre_suff1 = endsinArr(rv_txt.slice(0,-suf.length),pronoun_suf_pre1);
		var pre_suff2 = endsinArr(rv_txt.slice(0,-suf.length),pronoun_suf_pre2);	
		
		if (pre_suff1 != '') {
			token = token.slice(0,-suf.length);
		}
		if (pre_suff2 != '') {
			token = token.slice(0,  -suf.length)+ 'e';
		}
	}

	if (token != token_orig) {
		r1_txt = token.substring(r1);
		r2_txt = token.substring(r2);
		rv_txt = token.substring(rv);
	}

	var token_after0 = token;

	// Step 1:  Standard suffix removal
	
	if ((suf = endsinArr(r2_txt, new  Array('ativamente','abilamente','ivamente','osamente','icamente'))) != '') {
		token = token.slice(0, -suf.length);	// delete
	} else if ((suf = endsinArr(r2_txt, new  Array('icazione','icazioni','icatore','icatori','azione','azioni','atore','atori'))) != '') {
		token = token.slice(0,  -suf.length);	// delete
	} else if ((suf = endsinArr(r2_txt, new  Array('logia','logie'))) != '') {
		token = token.slice(0,  -suf.length)+ 'log'; // replace with log
	} else if ((suf =endsinArr(r2_txt, new  Array('uzione','uzioni','usione','usioni'))) != '') {
		token = token.slice(0,  -suf.length) + 'u'; // replace with u
	} else if ((suf = endsinArr(r2_txt, new  Array('enza','enze'))) != '') {
		token = token.slice(0,  -suf.length)+ 'ente'; // replace with ente
	} else if ((suf = endsinArr(rv_txt, new  Array('amento', 'amenti', 'imento', 'imenti'))) != '') {
		token = token.slice(0,  -suf.length);	// delete
	} else if ((suf = endsinArr(r1_txt, new  Array('amente'))) != '') {
		token = token.slice(0,  -suf.length); // delete
	} else if ((suf = endsinArr(r2_txt, new Array('atrice','atrici','abile','abili','ibile','ibili','mente','ante','anti','anza','anze
','iche','ichi','ismo','ismi','ista','iste','isti','istà','istè','istì','ico','ici','ica','ice','oso','osi','osa','ose'))) != '') {
		token = token.slice(0,  -suf.length); // delete
	} else if ((suf = endsinArr(r2_txt, new  Array('abilità', 'icità', 'ività', 'ità'))) != '') {
		token = ...
```
- example usage
```shell
...
'''javascript
var natural = require('natural');
'''

This example uses a Porter stemmer. "word" is returned.

'''javascript
console.log(natural.PorterStemmer.stem("words")); // stem a single word
'''

 in Russian:

'''javascript
console.log(natural.PorterStemmerRu.stem("падший"));
'''
...
```

#### <a name="apidoc.element.natural.PorterStemmerIt.tokenizeAndStem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerIt.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmerIt.tokenizeAndStem)
- description and source-code
```javascript
tokenizeAndStem = function (text, keepStops) {
    var stemmedTokens = [];

    new Tokenizer().tokenize(text).forEach(function(token) {
        if (keepStops || stopwords.words.indexOf(token) == -1) {
            var resultToken = token.toLowerCase();
            if (resultToken.match(/[a-zàèìòù0-9]/gi)) {
                resultToken = stemmer.stem(resultToken);
            }
            stemmedTokens.push(resultToken);
        }
    });

    return stemmedTokens;
}
```
- example usage
```shell
...

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
natural.LancasterStemmer.attach();
...
```



# <a name="apidoc.module.natural.PorterStemmerNo"></a>[module natural.PorterStemmerNo](#apidoc.module.natural.PorterStemmerNo)

#### <a name="apidoc.element.natural.PorterStemmerNo.addStopWord"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>addStopWord (stopWord)](#apidoc.element.natural.PorterStemmerNo.addStopWord)
- description and source-code
```javascript
addStopWord = function (stopWord) {
    stopwords.words.push(stopWord);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmerNo.addStopWords"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>addStopWords (moreStopWords)](#apidoc.element.natural.PorterStemmerNo.addStopWords)
- description and source-code
```javascript
addStopWords = function (moreStopWords) {
    stopwords.words = stopwords.words.concat(moreStopWords);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmerNo.attach"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>attach ()](#apidoc.element.natural.PorterStemmerNo.attach)
- description and source-code
```javascript
attach = function () {
    String.prototype.stem = function() {
        return stemmer.stem(this);
    };

    String.prototype.tokenizeAndStem = function(keepStops) {
        return stemmer.tokenizeAndStem(this, keepStops);
    };
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.PorterStemmerNo.getR1"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>getR1 (token)](#apidoc.element.natural.PorterStemmerNo.getR1)
- description and source-code
```javascript
function getR1(token) {
    var match = token.match(/[aeiouyæåø]{1}[^aeiouyæåø]([A-Za-z0-9_æøåÆØÅäÄöÖüÜ]+)/);

    if (match) {
        var preR1Length = match.index + 2;

        if (preR1Length < 3 && preR1Length > 0) {
            return token.slice(3);
        } else if (preR1Length >= 3) {
            return match[1];
        } else {
            return token;
        }
    }

    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmerNo.stem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>stem (token)](#apidoc.element.natural.PorterStemmerNo.stem)
- description and source-code
```javascript
stem = function (token) {
    return step3(step2(step1(token.toLowerCase()))).toString();
}
```
- example usage
```shell
...
'''javascript
var natural = require('natural');
'''

This example uses a Porter stemmer. "word" is returned.

'''javascript
console.log(natural.PorterStemmer.stem("words")); // stem a single word
'''

 in Russian:

'''javascript
console.log(natural.PorterStemmerRu.stem("падший"));
'''
...
```

#### <a name="apidoc.element.natural.PorterStemmerNo.step1"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>step1 (token)](#apidoc.element.natural.PorterStemmerNo.step1)
- description and source-code
```javascript
function step1(token) {
    // Perform step 1a-c
    var step1aResult = step1a(token),
        step1bResult = step1b(token),
        step1cResult = step1c(token);

    // Returne the shortest result string (from 1a, 1b and 1c)
    if (step1aResult.length < step1bResult.length) {
        return (step1aResult.length < step1cResult.length) ? step1aResult : step1cResult;
    } else {
        return (step1bResult.length < step1cResult.length) ? step1bResult : step1cResult;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmerNo.step1a"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>step1a (token)](#apidoc.element.natural.PorterStemmerNo.step1a)
- description and source-code
```javascript
function step1a(token) {
    var r1 = getR1(token);

    if (!r1) {
        return token;
    }

    var r1Match = r1.match(/(a|e|ede|ande|ende|ane|ene|hetene|en|heten|ar|er|heter|as|es|edes|endes|enes|hetenes|ens|hetens|ers|
ets|et|het|ast)$/);

    if (r1Match) {
        return token.replace(new RegExp(r1Match[1] + '$'), '');
    }

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmerNo.step1b"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>step1b (token)](#apidoc.element.natural.PorterStemmerNo.step1b)
- description and source-code
```javascript
function step1b(token) {
    var r1 = getR1(token);

    if (!r1) {
        return token;
    }

    if (token.match(/(b|c|d|f|g|h|j|l|m|n|o|p|r|t|v|y|z)s$/)) {
        return token.slice(0, -1);
    }

    if (token.match(/([^aeiouyæåø]k)s$/)) {
        return token.slice(0, -1);
    }

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmerNo.step1c"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>step1c (token)](#apidoc.element.natural.PorterStemmerNo.step1c)
- description and source-code
```javascript
function step1c(token) {
    var r1 = getR1(token);

    if (!r1) {
        return token;
    }

    if (r1.match(/(erte|ert)$/)) {
        return token.replace(/(erte|ert)$/, 'er');
    }

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmerNo.step2"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>step2 (token)](#apidoc.element.natural.PorterStemmerNo.step2)
- description and source-code
```javascript
function step2(token) {
    var r1 = getR1(token);

    if (!r1) {
        return token;
    }

    if (r1.match(/(d|v)t$/)) {
        return token.slice(0, -1);
    }

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmerNo.step3"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>step3 (token)](#apidoc.element.natural.PorterStemmerNo.step3)
- description and source-code
```javascript
function step3(token) {
    var r1 = getR1(token);

    if (!r1)
        return token;

    var r1Match = r1.match(/(leg|eleg|ig|eig|lig|elig|els|lov|elov|slov|hetslov)$/);

    if (r1Match) {
        return token.replace(new RegExp(r1Match[1] + '$'), '');
    }

    return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmerNo.tokenizeAndStem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerNo.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmerNo.tokenizeAndStem)
- description and source-code
```javascript
tokenizeAndStem = function (text, keepStops) {
    var stemmedTokens = [];

    new Tokenizer().tokenize(text).forEach(function(token) {
        if(keepStops || stopwords.words.indexOf(token.toLowerCase()) == -1)
            stemmedTokens.push(stemmer.stem(token));
    });

    return stemmedTokens;
}
```
- example usage
```shell
...

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
natural.LancasterStemmer.attach();
...
```



# <a name="apidoc.module.natural.PorterStemmerPt"></a>[module natural.PorterStemmerPt](#apidoc.module.natural.PorterStemmerPt)

#### <a name="apidoc.element.natural.PorterStemmerPt.addStopWords"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerPt.</span>addStopWords (words)](#apidoc.element.natural.PorterStemmerPt.addStopWords)
- description and source-code
```javascript
addStopWords = function (words) {
  stopwords.words = stopwords.words.concat(words);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.PorterStemmerPt.attach"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerPt.</span>attach ()](#apidoc.element.natural.PorterStemmerPt.attach)
- description and source-code
```javascript
attach = function () {
  String.prototype.stem = function () {
    return Stemmer.stem(this);
  };

  String.prototype.tokenizeAndStem = function (keepStops) {
    return Stemmer.tokenizeAndStem(this, keepStops);
  };
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.PorterStemmerPt.stem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerPt.</span>stem (word)](#apidoc.element.natural.PorterStemmerPt.stem)
- description and source-code
```javascript
stem = function (word) {
  var token = new Token(word.toLowerCase()),
    original;

  token = prelude(token);

  token.usingVowels('aeiouáéíóúâêôàãõ')
    .markRegion('all', 0)
    .markRegion('r1', null, markRegionN)
    .markRegion('r2', token.regions.r1, markRegionN)
    .markRegion('rv', null, markRegionV);

  original = token.string;

  // Always do step 1.
  token = standardSuffix(token);

  // Do step 2 if no ending was removed by step 1.
  if (token.string === original) {
    token = verbSuffix(token);
  }

  // If the last step to be obeyed — either step 1 or 2 — altered the word,
  // do step 3. Alternatively, if neither steps 1 nor 2 altered the word, do
  // step 4.
  token = token.string !== original ? iPrecededByCSuffix(token) : residualSuffix(token);

  // Always do step 5.
  token = residualForm(token);

  token = postlude(token);

  return token.string;
}
```
- example usage
```shell
...
'''javascript
var natural = require('natural');
'''

This example uses a Porter stemmer. "word" is returned.

'''javascript
console.log(natural.PorterStemmer.stem("words")); // stem a single word
'''

 in Russian:

'''javascript
console.log(natural.PorterStemmerRu.stem("падший"));
'''
...
```

#### <a name="apidoc.element.natural.PorterStemmerPt.tokenizeAndStem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerPt.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmerPt.tokenizeAndStem)
- description and source-code
```javascript
tokenizeAndStem = function (text, keepStops) {
  var stemmedTokens = [];

  var tokenStemmer = function (token) {
    if (keepStops || stopwords.words.indexOf(token.toLowerCase()) === -1) {
      stemmedTokens.push(Stemmer.stem(token));
    }
  };

  new Tokenizer().tokenize(text).forEach(tokenStemmer);

  return stemmedTokens;
}
```
- example usage
```shell
...

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
natural.LancasterStemmer.attach();
...
```



# <a name="apidoc.module.natural.PorterStemmerRu"></a>[module natural.PorterStemmerRu](#apidoc.module.natural.PorterStemmerRu)

#### <a name="apidoc.element.natural.PorterStemmerRu.attach"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerRu.</span>attach ()](#apidoc.element.natural.PorterStemmerRu.attach)
- description and source-code
```javascript
attach = function () {
    String.prototype.stem = function() {
        return stemmer.stem(this);
    };

    String.prototype.tokenizeAndStem = function(keepStops) {
        return stemmer.tokenizeAndStem(this, keepStops);
    };
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.PorterStemmerRu.stem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerRu.</span>stem (token)](#apidoc.element.natural.PorterStemmerRu.stem)
- description and source-code
```javascript
stem = function (token) {
	token = token.toLowerCase().replace(/ё/g, 'е');
	var volwesRegexp = /^(.*?[аеиоюяуыиэ])(.*)$/g;
	var RV = volwesRegexp.exec(token);
	if (!RV || RV.length < 3) {
		return token;
	}
	var head = RV[1];
	RV = RV[2];
	volwesRegexp.lastIndex = 0;
	var R2 = volwesRegexp.exec(RV);
	var result = perfectiveGerund(RV);
	if (result === null) {
		var resultReflexive = reflexive(RV) || RV;
		result = adjectival(resultReflexive);
		if (result === null) {
			result = verb(resultReflexive);
			if (result === null) {
				result = noun(resultReflexive);
				if (result === null) {
					result = resultReflexive;
				}
			}
		}
	}
	result = result.replace(/и$/g, '');
	var derivationalResult = result
	if (R2 && R2[2]) {
		derivationalResult = derivational(R2[2]);
		if (derivationalResult != null) {
			derivationalResult = derivational(result);
		} else {
			derivationalResult = result;
		}
	}

	var superlativeResult = superlative(derivationalResult) || derivationalResult;

	superlativeResult = superlativeResult.replace(/(н)н/g, '$1');
	superlativeResult = superlativeResult.replace(/ь$/g, '');
	return head + superlativeResult;
}
```
- example usage
```shell
...
'''javascript
var natural = require('natural');
'''

This example uses a Porter stemmer. "word" is returned.

'''javascript
console.log(natural.PorterStemmer.stem("words")); // stem a single word
'''

 in Russian:

'''javascript
console.log(natural.PorterStemmerRu.stem("падший"));
'''
...
```

#### <a name="apidoc.element.natural.PorterStemmerRu.tokenizeAndStem"></a>[function <span class="apidocSignatureSpan">natural.PorterStemmerRu.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.PorterStemmerRu.tokenizeAndStem)
- description and source-code
```javascript
tokenizeAndStem = function (text, keepStops) {
    var stemmedTokens = [];

    new Tokenizer().tokenize(text).forEach(function(token) {
        if (keepStops || stopwords.words.indexOf(token) == -1) {
            var resultToken = token.toLowerCase();
            if (resultToken.match(new RegExp('[а-яё0-9]+', 'gi'))) {
                resultToken = stemmer.stem(resultToken);
            }
            stemmedTokens.push(resultToken);
        }
    });

    return stemmedTokens;
}
```
- example usage
```shell
...

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
natural.LancasterStemmer.attach();
...
```



# <a name="apidoc.module.natural.PresentVerbInflector"></a>[module natural.PresentVerbInflector](#apidoc.module.natural.PresentVerbInflector)

#### <a name="apidoc.element.natural.PresentVerbInflector.PresentVerbInflector"></a>[function <span class="apidocSignatureSpan">natural.</span>PresentVerbInflector ()](#apidoc.element.natural.PresentVerbInflector.PresentVerbInflector)
- description and source-code
```javascript
PresentVerbInflector = function () {
    this.ambiguous = [
        'will'
    ];

    this.attach = attach;

    this.customPluralForms = [];
    this.customSingularForms = [];
    this.singularForms = new FormSet();
    this.pluralForms = new FormSet();

    this.addIrregular("am", "are");
    this.addIrregular("is", "are");
    this.addIrregular("was", "were");
    this.addIrregular("has", "have");

    this.singularForms.regularForms.push([/ed$/i, 'ed']);
    this.singularForms.regularForms.push([/ss$/i, 'sses']);
    this.singularForms.regularForms.push([/x$/i, 'xes']);
    this.singularForms.regularForms.push([/(h|z|o)$/i, '$1es']);
    this.singularForms.regularForms.push([/$zz/i, 'zzes']);
    this.singularForms.regularForms.push([/([^a|e|i|o|u])y$/i, '$1ies']);
    this.singularForms.regularForms.push([/$/i, 's']);

    this.pluralForms.regularForms.push([/sses$/i, 'ss']);
    this.pluralForms.regularForms.push([/xes$/i, 'x']);
    this.pluralForms.regularForms.push([/([cs])hes$/i, '$1h']);
    this.pluralForms.regularForms.push([/zzes$/i, 'zz']);
    this.pluralForms.regularForms.push([/([^h|z|o|i])es$/i, '$1e']);
    this.pluralForms.regularForms.push([/ies$/i, 'y']);//flies->fly
    this.pluralForms.regularForms.push([/e?s$/i, '']);
}
```
- example usage
```shell
...
### Present Tense Verbs

Present Tense Verbs can be pluralized/singularized with a PresentVerbInflector.
This feature is still experimental as of 0.0.42, so use with caution, and please
provide feedback.

'''javascript
var verbInflector = new natural.PresentVerbInflector();
'''

Outputs "becomes":

'''javascript
console.log(verbInflector.singularize('become'));
'''
...
```

#### <a name="apidoc.element.natural.PresentVerbInflector.super_"></a>[function <span class="apidocSignatureSpan">natural.PresentVerbInflector.</span>super_ ()](#apidoc.element.natural.PresentVerbInflector.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.RegexpTokenizer"></a>[module natural.RegexpTokenizer](#apidoc.module.natural.RegexpTokenizer)

#### <a name="apidoc.element.natural.RegexpTokenizer.RegexpTokenizer"></a>[function <span class="apidocSignatureSpan">natural.</span>RegexpTokenizer (options)](#apidoc.element.natural.RegexpTokenizer.RegexpTokenizer)
- description and source-code
```javascript
RegexpTokenizer = function (options) {
    var options = options || {};
    this._pattern = options.pattern || this._pattern;
    this.discardEmpty = options.discardEmpty || true;

    // Match and split on GAPS not the actual WORDS
    this._gaps = options.gaps;

    if (this._gaps === undefined) {
        this._gaps = true;
    }
}
```
- example usage
```shell
...
The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
console.log(tokenizer.tokenize("my dog hasn't any fleas."));
// [ 'my', 'dog', 'has', 'n\'t', 'any', 'fleas', '.' ]

tokenizer = new natural.RegexpTokenizer({pattern: /\-/});
console.log(tokenizer.tokenize("flea-dog"));
// [ 'flea', 'dog' ]

tokenizer = new natural.WordPunctTokenizer();
console.log(tokenizer.tokenize("my dog hasn't any fleas."));
// [ 'my',  'dog',  'hasn',  '\'',  't',  'any',  'fleas',  '.' ]
'''
...
```

#### <a name="apidoc.element.natural.RegexpTokenizer.super_"></a>[function <span class="apidocSignatureSpan">natural.RegexpTokenizer.</span>super_ ()](#apidoc.element.natural.RegexpTokenizer.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.RegexpTokenizer.prototype"></a>[module natural.RegexpTokenizer.prototype](#apidoc.module.natural.RegexpTokenizer.prototype)

#### <a name="apidoc.element.natural.RegexpTokenizer.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.RegexpTokenizer.prototype.</span>tokenize (s)](#apidoc.element.natural.RegexpTokenizer.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (s) {
    var results;

    if (this._gaps) {
        results = s.split(this._pattern);
        return (this.discardEmpty) ? _.without(results,'',' ') : results;
    } else {
        return s.match(this._pattern);
    }
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```



# <a name="apidoc.module.natural.SentenceAnalyzer"></a>[module natural.SentenceAnalyzer](#apidoc.module.natural.SentenceAnalyzer)

#### <a name="apidoc.element.natural.SentenceAnalyzer.SentenceAnalyzer"></a>[function <span class="apidocSignatureSpan">natural.</span>SentenceAnalyzer (pos, callback)](#apidoc.element.natural.SentenceAnalyzer.SentenceAnalyzer)
- description and source-code
```javascript
SentenceAnalyzer = function (pos, callback) {
    this.posObj = pos;
    this.senType = null;
    callback(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.SentenceAnalyzer.prototype"></a>[module natural.SentenceAnalyzer.prototype](#apidoc.module.natural.SentenceAnalyzer.prototype)

#### <a name="apidoc.element.natural.SentenceAnalyzer.prototype.implicitYou"></a>[function <span class="apidocSignatureSpan">natural.SentenceAnalyzer.prototype.</span>implicitYou ()](#apidoc.element.natural.SentenceAnalyzer.prototype.implicitYou)
- description and source-code
```javascript
implicitYou = function () {
    for (var i = 0; i < this.posObj.tags.length;i++) {
        if (this.posObj.tags[i].added) {
            return true;
        }
    }

    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SentenceAnalyzer.prototype.part"></a>[function <span class="apidocSignatureSpan">natural.SentenceAnalyzer.prototype.</span>part (callback)](#apidoc.element.natural.SentenceAnalyzer.prototype.part)
- description and source-code
```javascript
part = function (callback) {
    var subject = [],
	predicat = [],
	verbFound = false;
	
    this.prepositionPhrases();
	
    for (var i = 0; i < this.posObj.tags.length; i++) {
        if (this.posObj.tags[i].pos == "VB") {
            if (i === 0) {
                verbFound = true;
            } else {
                // We need to Test for any EX before the VB
                if (this.posObj.tags[i - 1].pos != "EX") {
                    verbFound = true;
                } else {
                    predicat.push(this.posObj.tags[i].token);
                }					
            }
        }

        // Add Pronoun Phrase (pp) Or Subject Phrase (sp)
        if (!verbFound) {
            if (this.posObj.tags[i].pp != true)
                this.posObj.tags[i].spos = "SP";

            subject.push(this.posObj.tags[i].token);
        } else {
            if (this.posObj.tags[i].pp != true)
                this.posObj.tags[i].spos = "PP";

            predicat.push(this.posObj.tags[i].token)
        }
    }
	
    if (subject.length == 0) {
	this.posObj.tags.push({token:"You",spos:"SP",pos:"PRP",added:true});
    }

    callback(this);	
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SentenceAnalyzer.prototype.predicateToString"></a>[function <span class="apidocSignatureSpan">natural.SentenceAnalyzer.prototype.</span>predicateToString ()](#apidoc.element.natural.SentenceAnalyzer.prototype.predicateToString)
- description and source-code
```javascript
predicateToString = function () {
    return this.posObj.tags.map(function(t){ if (t.spos == "PP" || t.spos == "P" ) return t.token }).join(' ');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SentenceAnalyzer.prototype.prepositionPhrases"></a>[function <span class="apidocSignatureSpan">natural.SentenceAnalyzer.prototype.</span>prepositionPhrases ()](#apidoc.element.natural.SentenceAnalyzer.prototype.prepositionPhrases)
- description and source-code
```javascript
prepositionPhrases = function () {
    var remove = false;

    for (var i = 0; i < this.posObj.tags.length; i++) {
        if (this.posObj.tags[i].pos.match("IN")) {
            remove = true;
        }

        if (remove) {
            this.posObj.tags[i].pp = true;
        }

        if (this.posObj.tags[i].pos.match("NN")) {
            remove = false;
        }
    }	
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SentenceAnalyzer.prototype.subjectToString"></a>[function <span class="apidocSignatureSpan">natural.SentenceAnalyzer.prototype.</span>subjectToString ()](#apidoc.element.natural.SentenceAnalyzer.prototype.subjectToString)
- description and source-code
```javascript
subjectToString = function () {
    return this.posObj.tags.map(function(t){ if (t.spos == "SP" || t.spos == "S" ) return t.token }).join(' ');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SentenceAnalyzer.prototype.toString"></a>[function <span class="apidocSignatureSpan">natural.SentenceAnalyzer.prototype.</span>toString ()](#apidoc.element.natural.SentenceAnalyzer.prototype.toString)
- description and source-code
```javascript
toString = function () {
    return this.posObj.tags.map(function(t){return t.token}).join(' ');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SentenceAnalyzer.prototype.type"></a>[function <span class="apidocSignatureSpan">natural.SentenceAnalyzer.prototype.</span>type (callback)](#apidoc.element.natural.SentenceAnalyzer.prototype.type)
- description and source-code
```javascript
type = function (callback) {
    var callback = callback || false;

    // Check for implicit you before popping a tag.
    var implicitYou = this.implicitYou();

    // FIXME - punct seems useless
    var lastElement = this.posObj.punct();
    lastElement = (lastElement.length != 0) ? lastElement.pop() : this.posObj.tags.pop();

    if (lastElement.pos !== ".") {
        if (implicitYou) {
            this.senType = "COMMAND";
        } else if (_(["WDT","WP","WP$","WRB"]).contains(this.posObj.tags[0].pos)) {
            // Sentences that start with: who, what where when why and how, then they are questions
            this.senType = "INTERROGATIVE";
        } else if (_(["PRP"]).contains(lastElement.pos)) {
            // Sentences that end in a Personal pronoun are most likely questions
            // eg. We should run away, should we [?]
            // eg. You want to see that again, do you [?]
            this.senType = "INTERROGATIVE";
        } else {
            this.senType = "UNKNOWN";
        }

    } else {
        switch(lastElement.token) {
            case "?": this.senType = "INTERROGATIVE"; break;
            case "!": this.senType = (implicitYou) ? "COMMAND":"EXCLAMATORY"; break;
            case ".": this.senType = (implicitYou) ? "COMMAND":"DECLARATIVE";	break;
        }
    }

    if (callback && _(callback).isFunction()) {
        callback(this);
    } else {
        return this.senType;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.SentenceTokenizer"></a>[module natural.SentenceTokenizer](#apidoc.module.natural.SentenceTokenizer)

#### <a name="apidoc.element.natural.SentenceTokenizer.SentenceTokenizer"></a>[function <span class="apidocSignatureSpan">natural.</span>SentenceTokenizer ()](#apidoc.element.natural.SentenceTokenizer.SentenceTokenizer)
- description and source-code
```javascript
SentenceTokenizer = function () {
    Tokenizer.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SentenceTokenizer.super_"></a>[function <span class="apidocSignatureSpan">natural.SentenceTokenizer.</span>super_ ()](#apidoc.element.natural.SentenceTokenizer.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.SentenceTokenizer.prototype"></a>[module natural.SentenceTokenizer.prototype](#apidoc.module.natural.SentenceTokenizer.prototype)

#### <a name="apidoc.element.natural.SentenceTokenizer.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.SentenceTokenizer.prototype.</span>tokenize (text)](#apidoc.element.natural.SentenceTokenizer.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (text) {
    // break string up in to sentences based on punctation and quotation marks
    var tokens = text.match(/([\"\'\‘\“\'\"\[\(\{\⟨][^\.\?\!]+[\.\?\!][\"\'\’\”\'\"\]\)\}\⟩]|[^\.\?\!]+[\.\?\!])\s?/g);

    // remove unecessary white space
    tokens = tokens.map(Function.prototype.call, String.prototype.trim);

    return this.trim(tokens);
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```



# <a name="apidoc.module.natural.ShortestPathTree"></a>[module natural.ShortestPathTree](#apidoc.module.natural.ShortestPathTree)

#### <a name="apidoc.element.natural.ShortestPathTree.ShortestPathTree"></a>[function <span class="apidocSignatureSpan">natural.</span>ShortestPathTree (digraph, start)](#apidoc.element.natural.ShortestPathTree.ShortestPathTree)
- description and source-code
```javascript
ShortestPathTree = function (digraph, start) {
    var _this = this;
    this.edgeTo = [];
    this.distTo = [];
    this.distTo[start] = 0.0;
    this.start = start;
    this.top = new Topological(digraph);
    this.top.order().forEach(function(vertex){
        _this.relaxVertex(digraph, vertex, _this);
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.ShortestPathTree.prototype"></a>[module natural.ShortestPathTree.prototype](#apidoc.module.natural.ShortestPathTree.prototype)

#### <a name="apidoc.element.natural.ShortestPathTree.prototype.getDistTo"></a>[function <span class="apidocSignatureSpan">natural.ShortestPathTree.prototype.</span>getDistTo (v)](#apidoc.element.natural.ShortestPathTree.prototype.getDistTo)
- description and source-code
```javascript
getDistTo = function (v) {
    return this.distTo[v];
}
```
- example usage
```shell
...
digraph is an instance of EdgeWeightedDigraph, the second param is the start vertex of DAG.

### getDistTo(vertex)

Will return the dist to vertex.

'''javascript
console.log(spt.getDistTo(4));
'''
the output will be: 0.35

### hasDistTo(vertex)

'''javascript
console.log(spt.hasDistTo(4));
...
```

#### <a name="apidoc.element.natural.ShortestPathTree.prototype.hasPathTo"></a>[function <span class="apidocSignatureSpan">natural.ShortestPathTree.prototype.</span>hasPathTo (v)](#apidoc.element.natural.ShortestPathTree.prototype.hasPathTo)
- description and source-code
```javascript
hasPathTo = function (v) {
    var dist = this.distTo[v];
    if(v == this.start) return false;
    return /\d/.test(dist) ? dist != Number.MAX_VALUE : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.ShortestPathTree.prototype.pathTo"></a>[function <span class="apidocSignatureSpan">natural.ShortestPathTree.prototype.</span>pathTo (v)](#apidoc.element.natural.ShortestPathTree.prototype.pathTo)
- description and source-code
```javascript
pathTo = function (v) {
    if (!this.hasPathTo(v) || v == this.start) return [];
    var path = [];
    var edgeTo = this.edgeTo;
    for (var e = edgeTo[v]; !!e; e = edgeTo[e.from()]) {
        path.push(e.to());
    }
    path.push(this.start);
    return path.reverse();
}
```
- example usage
```shell
...
false
'''

### pathTo(vertex)
this will return a shortest path:

'''javascript
console.log(spt.pathTo(4));
'''

output will be:

'''javascript
[5, 4]
'''
...
```

#### <a name="apidoc.element.natural.ShortestPathTree.prototype.relaxEdge"></a>[function <span class="apidocSignatureSpan">natural.ShortestPathTree.prototype.</span>relaxEdge (e)](#apidoc.element.natural.ShortestPathTree.prototype.relaxEdge)
- description and source-code
```javascript
relaxEdge = function (e) {
    var distTo = this.distTo,
        edgeTo = this.edgeTo;
    var v = e.from(), w = e.to();
    if (distTo[w] > distTo[v] + e.weight) {
        distTo[w] = distTo[v] + e.weight;
        edgeTo[w] = e;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.ShortestPathTree.prototype.relaxVertex"></a>[function <span class="apidocSignatureSpan">natural.ShortestPathTree.prototype.</span>relaxVertex (digraph, vertex, tree)](#apidoc.element.natural.ShortestPathTree.prototype.relaxVertex)
- description and source-code
```javascript
relaxVertex = function (digraph, vertex, tree) {
    var distTo = tree.distTo;
    var edgeTo = tree.edgeTo;
    digraph.getAdj(vertex).forEach(function(edge){
        var w = edge.to();
        distTo[w] = /\d/.test(distTo[w]) ? distTo[w] : Number.MAX_VALUE;
        distTo[vertex] = distTo[vertex] || 0;
        if (distTo[w] > distTo[vertex] + edge.weight) {
            // in case of the result of 0.28+0.34 is 0.62000001
            distTo[w] = parseFloat((distTo[vertex] + edge.weight).toFixed(2));
            edgeTo[w] = edge;
        }
    });

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.SoundEx"></a>[module natural.SoundEx](#apidoc.module.natural.SoundEx)

#### <a name="apidoc.element.natural.SoundEx.attach"></a>[function <span class="apidocSignatureSpan">natural.SoundEx.</span>attach ()](#apidoc.element.natural.SoundEx.attach)
- description and source-code
```javascript
attach = function () {
	var phonetic = this;

    String.prototype.soundsLike = function(compareTo) {
        return phonetic.compare(this, compareTo);
    }

    String.prototype.phonetics = function() {
        return phonetic.process(this);
    }
	
    String.prototype.tokenizeAndPhoneticize = function(keepStops) {
        var phoneticizedTokens = [];

        tokenizer.tokenize(this).forEach(function(token) {
            if(keepStops || stopwords.words.indexOf(token) < 0)
                phoneticizedTokens.push(token.phonetics());
        });

        return phoneticizedTokens;
    }
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.SoundEx.compare"></a>[function <span class="apidocSignatureSpan">natural.SoundEx.</span>compare (stringA, stringB)](#apidoc.element.natural.SoundEx.compare)
- description and source-code
```javascript
compare = function (stringA, stringB) {
    return this.process(stringA) == this.process(stringB);
}
```
- example usage
```shell
...
var wordA = 'phonetics';
var wordB = 'fonetix';
'''

To test the two words to see if they sound alike:

'''javascript
if(metaphone.compare(wordA, wordB))
    console.log('they sound alike!');
'''

The raw phonetics are obtained with 'process()':

'''javascript
console.log(metaphone.process('phonetics'));
...
```

#### <a name="apidoc.element.natural.SoundEx.condense"></a>[function <span class="apidocSignatureSpan">natural.SoundEx.</span>condense (token)](#apidoc.element.natural.SoundEx.condense)
- description and source-code
```javascript
function condense(token) {
    return token.replace(/(\d)?\1+/g, '$1');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SoundEx.padRight0"></a>[function <span class="apidocSignatureSpan">natural.SoundEx.</span>padRight0 (token)](#apidoc.element.natural.SoundEx.padRight0)
- description and source-code
```javascript
function padRight0(token) {
    if(token.length < 4)
        return token + Array(4 - token.length).join('0');
    else
        return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SoundEx.process"></a>[function <span class="apidocSignatureSpan">natural.SoundEx.</span>process (token, maxLength)](#apidoc.element.natural.SoundEx.process)
- description and source-code
```javascript
process = function (token, maxLength) {
    token = token.toLowerCase();
    var transformed = condense(transform(token.substr(1, token.length - 1))); // anything that isn't a digit goes
    // deal with duplicate INITIAL consonant SOUNDS
    transformed = transformed.replace(new RegExp("^" + transform(token.charAt(0))), '');
    return token.charAt(0).toUpperCase() + padRight0(transformed.replace(/\D/g, '')).substr(0, (maxLength && maxLength - 1) || 3
);
}
```
- example usage
```shell
...
if(metaphone.compare(wordA, wordB))
    console.log('they sound alike!');
'''

The raw phonetics are obtained with 'process()':

'''javascript
console.log(metaphone.process('phonetics'));
'''

A maximum code length can be supplied:

'''javascript
console.log(metaphone.process('phonetics', 3));
'''
...
```

#### <a name="apidoc.element.natural.SoundEx.transformHum"></a>[function <span class="apidocSignatureSpan">natural.SoundEx.</span>transformHum (token)](#apidoc.element.natural.SoundEx.transformHum)
- description and source-code
```javascript
function transformHum(token) {
    return token.replace(/[mn]/g, '5');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SoundEx.transformL"></a>[function <span class="apidocSignatureSpan">natural.SoundEx.</span>transformL (token)](#apidoc.element.natural.SoundEx.transformL)
- description and source-code
```javascript
function transformL(token) {
    return token.replace(/l/g, '4');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SoundEx.transformLipps"></a>[function <span class="apidocSignatureSpan">natural.SoundEx.</span>transformLipps (token)](#apidoc.element.natural.SoundEx.transformLipps)
- description and source-code
```javascript
function transformLipps(token) {
    return token.replace(/[bfpv]/g, '1');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SoundEx.transformR"></a>[function <span class="apidocSignatureSpan">natural.SoundEx.</span>transformR (token)](#apidoc.element.natural.SoundEx.transformR)
- description and source-code
```javascript
function transformR(token) {
    return token.replace(/r/g, '6');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SoundEx.transformThroats"></a>[function <span class="apidocSignatureSpan">natural.SoundEx.</span>transformThroats (token)](#apidoc.element.natural.SoundEx.transformThroats)
- description and source-code
```javascript
function transformThroats(token) {
    return token.replace(/[cgjkqsxz]/g, '2');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.SoundEx.transformToungue"></a>[function <span class="apidocSignatureSpan">natural.SoundEx.</span>transformToungue (token)](#apidoc.element.natural.SoundEx.transformToungue)
- description and source-code
```javascript
function transformToungue(token) {
    return token.replace(/[dt]/g, '3');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.SoundExDM"></a>[module natural.SoundExDM](#apidoc.module.natural.SoundExDM)

#### <a name="apidoc.element.natural.SoundExDM.attach"></a>[function <span class="apidocSignatureSpan">natural.SoundExDM.</span>attach ()](#apidoc.element.natural.SoundExDM.attach)
- description and source-code
```javascript
attach = function () {
	var phonetic = this;

    String.prototype.soundsLike = function(compareTo) {
        return phonetic.compare(this, compareTo);
    }

    String.prototype.phonetics = function() {
        return phonetic.process(this);
    }
	
    String.prototype.tokenizeAndPhoneticize = function(keepStops) {
        var phoneticizedTokens = [];

        tokenizer.tokenize(this).forEach(function(token) {
            if(keepStops || stopwords.words.indexOf(token) < 0)
                phoneticizedTokens.push(token.phonetics());
        });

        return phoneticizedTokens;
    }
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.SoundExDM.compare"></a>[function <span class="apidocSignatureSpan">natural.SoundExDM.</span>compare (stringA, stringB)](#apidoc.element.natural.SoundExDM.compare)
- description and source-code
```javascript
compare = function (stringA, stringB) {
    return this.process(stringA) == this.process(stringB);
}
```
- example usage
```shell
...
var wordA = 'phonetics';
var wordB = 'fonetix';
'''

To test the two words to see if they sound alike:

'''javascript
if(metaphone.compare(wordA, wordB))
    console.log('they sound alike!');
'''

The raw phonetics are obtained with 'process()':

'''javascript
console.log(metaphone.process('phonetics'));
...
```

#### <a name="apidoc.element.natural.SoundExDM.process"></a>[function <span class="apidocSignatureSpan">natural.SoundExDM.</span>process (word, codeLength)](#apidoc.element.natural.SoundExDM.process)
- description and source-code
```javascript
function process(word, codeLength) {
	codeLength = codeLength || 6;
    word = word.toUpperCase();
    var output = '';

    var pos = 0, lastCode = -1;
    while (pos < word.length) {
        var substr = word.slice(pos);
        var rules = findRules(substr);

        var code;
        if (pos == 0) {
            // at the beginning of the word
            code = rules.mapping[0];
        } else if (substr[rules.length] && findRules(substr[rules.length]).mapping[0] == 0) {
            // before a vowel
            code = rules.mapping[1];
        } else {
            // any other situation
            code = rules.mapping[2];
        }

        if ((code != -1) && (code != lastCode)) output += code;
        lastCode = code;
        pos += rules.length;

    }

    return normalizeLength(output, codeLength);
}
```
- example usage
```shell
...
if(metaphone.compare(wordA, wordB))
    console.log('they sound alike!');
'''

The raw phonetics are obtained with 'process()':

'''javascript
console.log(metaphone.process('phonetics'));
'''

A maximum code length can be supplied:

'''javascript
console.log(metaphone.process('phonetics', 3));
'''
...
```



# <a name="apidoc.module.natural.Spellcheck"></a>[module natural.Spellcheck](#apidoc.module.natural.Spellcheck)

#### <a name="apidoc.element.natural.Spellcheck.Spellcheck"></a>[function <span class="apidocSignatureSpan">natural.</span>Spellcheck (wordlist)](#apidoc.element.natural.Spellcheck.Spellcheck)
- description and source-code
```javascript
function Spellcheck(wordlist) {
    this.trie = new Trie();
    this.trie.addStrings(wordlist);
    this.word2frequency = {};
    for(var i in wordlist) {
        if(!this.word2frequency[wordlist[i]]) {
            this.word2frequency[wordlist[i]] = 0;
        }
        this.word2frequency[wordlist[i]]++;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.Spellcheck.prototype"></a>[module natural.Spellcheck.prototype](#apidoc.module.natural.Spellcheck.prototype)

#### <a name="apidoc.element.natural.Spellcheck.prototype.edits"></a>[function <span class="apidocSignatureSpan">natural.Spellcheck.prototype.</span>edits (word)](#apidoc.element.natural.Spellcheck.prototype.edits)
- description and source-code
```javascript
edits = function (word) {
    var alphabet = 'abcdefghijklmnopqrstuvwxyz';
    var edits = [];
    for(var i=0; i<word.length+1; i++) {
        if(i>0) edits.push(word.slice(0,i-1)+word.slice(i,word.length)); // deletes
        if(i>0 && i<word.length+1) edits.push(word.slice(0,i-1) + word.slice(i,i+1) + word.slice(i-1, i) + word.slice(i+1,word.length
)); // transposes
        for(var k=0; k<alphabet.length; k++) {
            if(i>0) edits.push(word.slice(0,i-1)+alphabet[k]+word.slice(i,word.length)); // replaces
            edits.push(word.slice(0,i)+alphabet[k]+word.slice(i,word.length)); // inserts
        }
    }
    // Deduplicate edits
    edits = edits.filter(function (v, i, a) { return a.indexOf(v) == i });
    return edits;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Spellcheck.prototype.editsWithMaxDistance"></a>[function <span class="apidocSignatureSpan">natural.Spellcheck.prototype.</span>editsWithMaxDistance (word, distance)](#apidoc.element.natural.Spellcheck.prototype.editsWithMaxDistance)
- description and source-code
```javascript
editsWithMaxDistance = function (word, distance) {
    return this.editsWithMaxDistanceHelper(distance, [[word]]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Spellcheck.prototype.editsWithMaxDistanceHelper"></a>[function <span class="apidocSignatureSpan">natural.Spellcheck.prototype.</span>editsWithMaxDistanceHelper (distanceCounter, distance2edits)](#apidoc.element.natural.Spellcheck.prototype.editsWithMaxDistanceHelper)
- description and source-code
```javascript
editsWithMaxDistanceHelper = function (distanceCounter, distance2edits) {
    if(distanceCounter == 0) return distance2edits;
    var currentDepth = distance2edits.length-1;
    var words = distance2edits[currentDepth];
    var edits = this.edits(words[0]);
    distance2edits[currentDepth+1] = [];
    for(var i in words) {
        distance2edits[currentDepth+1] = distance2edits[currentDepth+1].concat(this.edits(words[i]));
    }
    return this.editsWithMaxDistanceHelper(distanceCounter-1, distance2edits);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Spellcheck.prototype.getCorrections"></a>[function <span class="apidocSignatureSpan">natural.Spellcheck.prototype.</span>getCorrections (word, maxDistance)](#apidoc.element.natural.Spellcheck.prototype.getCorrections)
- description and source-code
```javascript
getCorrections = function (word, maxDistance) {
    var self = this;
    if(!maxDistance) maxDistance = 1;
    var edits = this.editsWithMaxDistance(word, maxDistance);
    edits = edits.slice(1,edits.length);
    edits = edits.map(function(editList) {
       return editList.filter(function(word) { return self.isCorrect(word); })
                      .map(function(word) { return [word, self.word2frequency[word]]; })
                      .sort(function(a,b) { return a[1] > b[1] ? -1 : 1; })
                      .map(function(wordscore) { return wordscore[0]; });
    });
    var flattened = [];
    for(var i in edits) {
        if(edits[i].length) flattened = flattened.concat(edits[i]);
    }
    return flattened.filter(function (v, i, a) { return a.indexOf(v) == i });
}
```
- example usage
```shell
...
'''javascript
spellcheck.isCorrect('cat'); // false
'''

It suggests corrections (sorted by probability in descending order) that are up to a maximum edit distance away from the input word
. According to Norvig, a max distance of 1 will cover 80% to 95% of spelling mistakes. After a distance of 2, it becomes very slow
.

'''javascript
spellcheck.getCorrections('soemthing', 1); // ['something']
spellcheck.getCorrections('soemthing', 2); // ['something', 'soothing']
'''

## POS Tagger

This is a part-of-speech tagger based on Eric Brill's transformational
algorithm. Transformation rules are specified in external files.
...
```

#### <a name="apidoc.element.natural.Spellcheck.prototype.isCorrect"></a>[function <span class="apidocSignatureSpan">natural.Spellcheck.prototype.</span>isCorrect (word)](#apidoc.element.natural.Spellcheck.prototype.isCorrect)
- description and source-code
```javascript
isCorrect = function (word) {
    return this.trie.contains(word);
}
```
- example usage
```shell
...
var corpus = ['something', 'soothing'];
var spellcheck = new Spellcheck(corpus);
'''

It uses the trie datastructure for fast boolean lookup of a word

'''javascript
spellcheck.isCorrect('cat'); // false
'''

It suggests corrections (sorted by probability in descending order) that are up to a maximum edit distance away from the input word
. According to Norvig, a max distance of 1 will cover 80% to 95% of spelling mistakes. After a distance of 2, it becomes very slow
.

'''javascript
spellcheck.getCorrections('soemthing', 1); // ['something']
spellcheck.getCorrections('soemthing', 2); // ['something', 'soothing']
...
```



# <a name="apidoc.module.natural.StemmerJa"></a>[module natural.StemmerJa](#apidoc.module.natural.StemmerJa)

#### <a name="apidoc.element.natural.StemmerJa.StemmerJa"></a>[function <span class="apidocSignatureSpan">natural.</span>StemmerJa ()](#apidoc.element.natural.StemmerJa.StemmerJa)
- description and source-code
```javascript
StemmerJa = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.StemmerJa.prototype"></a>[module natural.StemmerJa.prototype](#apidoc.module.natural.StemmerJa.prototype)

#### <a name="apidoc.element.natural.StemmerJa.prototype.attach"></a>[function <span class="apidocSignatureSpan">natural.StemmerJa.prototype.</span>attach ()](#apidoc.element.natural.StemmerJa.prototype.attach)
- description and source-code
```javascript
attach = function () {
  var self = this;

  String.prototype.stem = function() {
    return self.stem(this);
  };

  String.prototype.tokenizeAndStem = function(keepStops) {
    return self.tokenizeAndStem(this, keepStops);
  };
}
```
- example usage
```shell
...
'''

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
...
```

#### <a name="apidoc.element.natural.StemmerJa.prototype.isKatakana"></a>[function <span class="apidocSignatureSpan">natural.StemmerJa.prototype.</span>isKatakana (str)](#apidoc.element.natural.StemmerJa.prototype.isKatakana)
- description and source-code
```javascript
isKatakana = function (str) {
  return !!str.match(/^[゠-ヿ]+$/);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.StemmerJa.prototype.stem"></a>[function <span class="apidocSignatureSpan">natural.StemmerJa.prototype.</span>stem (token)](#apidoc.element.natural.StemmerJa.prototype.stem)
- description and source-code
```javascript
stem = function (token) {
  token = this.stemKatakana(token);

  return token;
}
```
- example usage
```shell
...
'''javascript
var natural = require('natural');
'''

This example uses a Porter stemmer. "word" is returned.

'''javascript
console.log(natural.PorterStemmer.stem("words")); // stem a single word
'''

 in Russian:

'''javascript
console.log(natural.PorterStemmerRu.stem("падший"));
'''
...
```

#### <a name="apidoc.element.natural.StemmerJa.prototype.stemKatakana"></a>[function <span class="apidocSignatureSpan">natural.StemmerJa.prototype.</span>stemKatakana (token)](#apidoc.element.natural.StemmerJa.prototype.stemKatakana)
- description and source-code
```javascript
stemKatakana = function (token) {
  var HIRAGANA_KATAKANA_PROLONGED_SOUND_MARK = 'ー';
  var DEFAULT_MINIMUM_LENGTH = 4;

  if (token.length >= DEFAULT_MINIMUM_LENGTH
      && token.slice(-1) === HIRAGANA_KATAKANA_PROLONGED_SOUND_MARK
      && this.isKatakana(token)) {
    token = token.slice(0, token.length - 1);
  }
  return token;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.StemmerJa.prototype.tokenizeAndStem"></a>[function <span class="apidocSignatureSpan">natural.StemmerJa.prototype.</span>tokenizeAndStem (text, keepStops)](#apidoc.element.natural.StemmerJa.prototype.tokenizeAndStem)
- description and source-code
```javascript
tokenizeAndStem = function (text, keepStops) {
  var self = this;
  var stemmedTokens = [];
  var tokens = new Tokenizer().tokenize(text);

  // This is probably faster than an if at each iteration.
  if (keepStops) {
    tokens.forEach(function(token) {
      var resultToken = token.toLowerCase();
      resultToken = self.stem(resultToken);
      stemmedTokens.push(resultToken);
    });
  } else {
    tokens.forEach(function(token) {
      if (stopwords.indexOf(token) == -1) {
        var resultToken = token.toLowerCase();
        resultToken = self.stem(resultToken);
        stemmedTokens.push(resultToken);
      }
    });
  }

  return stemmedTokens;
}
```
- example usage
```shell
...

'attach()' patches 'stem()' and 'tokenizeAndStem()' to String as a shortcut to
'PorterStemmer.stem(token)'. 'tokenizeAndStem()' breaks text up into single words
and returns an array of stemmed tokens.

'''javascript
natural.PorterStemmer.attach();
console.log("i am waking up to the sounds of chainsaws".tokenizeAndStem());
console.log("chainsaws".stem());
'''

the same thing can be done with a Lancaster stemmer:

'''javascript
natural.LancasterStemmer.attach();
...
```



# <a name="apidoc.module.natural.TfIdf"></a>[module natural.TfIdf](#apidoc.module.natural.TfIdf)

#### <a name="apidoc.element.natural.TfIdf.TfIdf"></a>[function <span class="apidocSignatureSpan">natural.</span>TfIdf (deserialized)](#apidoc.element.natural.TfIdf.TfIdf)
- description and source-code
```javascript
function TfIdf(deserialized) {
    if(deserialized)
        this.documents = deserialized.documents;
    else
        this.documents = [];

    this._idfCache = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.TfIdf.tf"></a>[function <span class="apidocSignatureSpan">natural.TfIdf.</span>tf (term, document)](#apidoc.element.natural.TfIdf.tf)
- description and source-code
```javascript
function tf(term, document) {
    return document[term] ? document[term]: 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.TfIdf.prototype"></a>[module natural.TfIdf.prototype](#apidoc.module.natural.TfIdf.prototype)

#### <a name="apidoc.element.natural.TfIdf.prototype.addDocument"></a>[function <span class="apidocSignatureSpan">natural.TfIdf.prototype.</span>addDocument (document, key, restoreCache)](#apidoc.element.natural.TfIdf.prototype.addDocument)
- description and source-code
```javascript
addDocument = function (document, key, restoreCache) {
    this.documents.push(buildDocument(document, key));

    // make sure the cache is invalidated when new documents arrive
    if(restoreCache === true) {
        for(var term in this._idfCache) {
            // invoking idf with the force option set will
            // force a recomputation of the idf, and it will
            // automatically refresh the cache value.
            this.idf(term, true);
        }
    }   else {
        this._idfCache = {};
    }
}
```
- example usage
```shell
...
  classifier = new natural.BayesClassifier();
'''

You can train the classifier on sample text. It will use reasonable defaults to
tokenize and stem the text.

'''javascript
classifier.addDocument('i am long qqqq', 'buy');
classifier.addDocument('buy the q\'s', 'buy');
classifier.addDocument('short gold', 'sell');
classifier.addDocument('sell gold', 'sell');

classifier.train();
'''
...
```

#### <a name="apidoc.element.natural.TfIdf.prototype.addFileSync"></a>[function <span class="apidocSignatureSpan">natural.TfIdf.prototype.</span>addFileSync (path, encoding, key, restoreCache)](#apidoc.element.natural.TfIdf.prototype.addFileSync)
- description and source-code
```javascript
addFileSync = function (path, encoding, key, restoreCache) {
    if(!encoding)
        encoding = 'utf8';
    if(!isEncoding(encoding))
        throw new Error('Invalid encoding: ' + encoding);

    var document = fs.readFileSync(path, encoding);
    this.documents.push(buildDocument(document, key));

    // make sure the cache is invalidated when new documents arrive
    if(restoreCache === true) {
        for(var term in this._idfCache) {
            // invoking idf with the force option set will
            // force a recomputation of the idf, and it will
            // automatically refresh the cache value.
            this.idf(term, true);
        }
    }
    else {
        this._idfCache = {};
    }
}
```
- example usage
```shell
...
console.log(tfidf.tfidf('node', 1));
'''

A TfIdf instance can also load documents from files on disk.

'''javascript
var tfidf = new TfIdf();
tfidf.addFileSync('data_files/one.txt');
tfidf.addFileSync('data_files/two.txt');
'''

Multiple terms can be measured as well, with their weights being added into
a single measure value. The following example determines that the last document
is the most relevant to the words "node" and "ruby".
...
```

#### <a name="apidoc.element.natural.TfIdf.prototype.idf"></a>[function <span class="apidocSignatureSpan">natural.TfIdf.prototype.</span>idf (term, force)](#apidoc.element.natural.TfIdf.prototype.idf)
- description and source-code
```javascript
idf = function (term, force) {

    // Lookup the term in the New term-IDF caching,
    // this will cut search times down exponentially on large document sets.
    if(this._idfCache[term] && this._idfCache.hasOwnProperty(term) && force !== true)
        return this._idfCache[term];

    var docsWithTerm = this.documents.reduce(function(count, document) {
        return count + (documentHasTerm(term, document) ? 1 : 0);
    }, 0);

    var idf = 1 + Math.log((this.documents.length) / ( 1 + docsWithTerm ));

    // Add the idf to the term cache and return it
    this._idfCache[term] = idf;
    return idf;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.TfIdf.prototype.listTerms"></a>[function <span class="apidocSignatureSpan">natural.TfIdf.prototype.</span>listTerms (d)](#apidoc.element.natural.TfIdf.prototype.listTerms)
- description and source-code
```javascript
listTerms = function (d) {
    var terms = [];

    for(var term in this.documents[d]) {
        if(term != '__key')
           terms.push({term: term, tfidf: this.tfidf(term, d)});
    }

    return terms.sort(function(x, y) { return y.tfidf - x.tfidf; });
}
```
- example usage
```shell
...
});
'''

It's possible to retrieve a list of all terms in a document, sorted by their
importance.

'''javascript
tfidf.listTerms(0 /*document index*/).forEach(function(item) {
    console.log(item.term + ': ' + item.tfidf);
});
'''

A TfIdf instance can also be serialized and deserialized for save and recall.

'''javascript
...
```

#### <a name="apidoc.element.natural.TfIdf.prototype.setTokenizer"></a>[function <span class="apidocSignatureSpan">natural.TfIdf.prototype.</span>setTokenizer (t)](#apidoc.element.natural.TfIdf.prototype.setTokenizer)
- description and source-code
```javascript
setTokenizer = function (t) {
    if(!_.isFunction(t.tokenize))
        throw new Error('Expected a valid Tokenizer');
    tokenizer = t;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.TfIdf.prototype.tfidf"></a>[function <span class="apidocSignatureSpan">natural.TfIdf.prototype.</span>tfidf (terms, d)](#apidoc.element.natural.TfIdf.prototype.tfidf)
- description and source-code
```javascript
tfidf = function (terms, d) {
    var _this = this;

    if(!_.isArray(terms))
        terms = tokenizer.tokenize(terms.toString().toLowerCase());

    return terms.reduce(function(value, term) {
        var idf = _this.idf(term);
        idf = idf === Infinity ? 0 : idf;
        return value + (tf(term, _this.documents[d]) * idf);
    }, 0.0);
}
```
- example usage
```shell
...
'''

This approach can also be applied to individual documents.

The following example measures the term "node" in the first and second documents.

'''javascript
console.log(tfidf.tfidf('node', 0));
console.log(tfidf.tfidf('node', 1));
'''

A TfIdf instance can also load documents from files on disk.

'''javascript
var tfidf = new TfIdf();
...
```

#### <a name="apidoc.element.natural.TfIdf.prototype.tfidfs"></a>[function <span class="apidocSignatureSpan">natural.TfIdf.prototype.</span>tfidfs (terms, callback)](#apidoc.element.natural.TfIdf.prototype.tfidfs)
- description and source-code
```javascript
tfidfs = function (terms, callback) {
    var tfidfs = new Array(this.documents.length);

    for(var i = 0; i < this.documents.length; i++) {
        tfidfs[i] = this.tfidf(terms, i);

        if(callback)
            callback(i, tfidfs[i], this.documents[i].__key);
    }

    return tfidfs;
}
```
- example usage
```shell
...

tfidf.addDocument('this document is about node.');
tfidf.addDocument('this document is about ruby.');
tfidf.addDocument('this document is about ruby and node.');
tfidf.addDocument('this document is about node. it has node examples');

console.log('node --------------------------------');
tfidf.tfidfs('node', function(i, measure) {
    console.log('document #' + i + ' is ' + measure);
});

console.log('ruby --------------------------------');
tfidf.tfidfs('ruby', function(i, measure) {
    console.log('document #' + i + ' is ' + measure);
});
...
```



# <a name="apidoc.module.natural.TokenizerJa"></a>[module natural.TokenizerJa](#apidoc.module.natural.TokenizerJa)

#### <a name="apidoc.element.natural.TokenizerJa.TokenizerJa"></a>[function <span class="apidocSignatureSpan">natural.</span>TokenizerJa ()](#apidoc.element.natural.TokenizerJa.TokenizerJa)
- description and source-code
```javascript
TokenizerJa = function () {
  this.chartype_ = [
    [/[〇一二三四五六七八九十百千万億兆]/, 'M'],
    [/[一-鿌〆]/, 'H'],
    [/[ぁ-ゟ]/, 'I'],
    [/[゠-ヿ]/, 'K'],
    [/[a-zA-Z]/, 'A'],
    [/[0-9]/, 'N']
  ];

  this.BIAS__ = -332;
  this.BC1__ = {'HH': 6, 'II': 2461, 'KH': 406, 'OH': -1378};
  this.BC2__ = {'AA': -3267, 'AI': 2744, 'AN': -878, 'HH': -4070, 'HM': -1711, 'HN': 4012, 'HO': 3761, 'IA': 1327, 'IH': -1184, '
II': -1332, 'IK': 1721, 'IO': 5492, 'KI': 3831, 'KK': -8741, 'MH': -3132, 'MK': 3334, 'OO': -2920};
  this.BC3__ = {'HH': 996, 'HI': 626, 'HK': -721, 'HN': -1307, 'HO': -836, 'IH': -301, 'KK': 2762, 'MK': 1079, 'MM': 4034, 'OA': -
1652, 'OH': 266};
  this.BP1__ = {'BB': 295, 'OB': 304, 'OO': -125, 'UB': 352};
  this.BP2__ = {'BO': 60, 'OO': -1762};
  this.BQ1__ = {'BHH': 1150, 'BHM': 1521, 'BII': -1158, 'BIM': 886, 'BMH': 1208, 'BNH': 449, 'BOH': -91, 'BOO': -2597, 'OHI': 451
, 'OIH': -296, 'OKA': 1851, 'OKH': -1020, 'OKK': 904, 'OOO': 2965};
  this.BQ2__ = {'BHH': 118, 'BHI': -1159, 'BHM': 466, 'BIH': -919, 'BKK': -1720, 'BKO': 864, 'OHH': -1139, 'OHM': -181, 'OIH': 153
, 'UHI': -1146};
  this.BQ3__ = {'BHH': -792, 'BHI': 2664, 'BII': -299, 'BKI': 419, 'BMH': 937, 'BMM': 8335, 'BNN': 998, 'BOH': 775, 'OHH': 2174, '
OHM': 439, 'OII': 280, 'OKH': 1798, 'OKI': -793, 'OKO': -2242, 'OMH': -2402, 'OOO': 11699};
  this.BQ4__ = {'BHH': -3895, 'BIH': 3761, 'BII': -4654, 'BIK': 1348, 'BKK': -1806, 'BMI': -3385, 'BOO': -12396, 'OAH': 926, 'OHH
': 266, 'OHK': -2036, 'ONN': -973};
  this.BW1__ = {'，と': 660, '，同': 727, 'B1あ': 1404, 'B1同': 542, '、と': 660, '、同': 727, '｣と': 1682, 'あっ': 1505, 'いう': 1743, 'いっ': -
2055, 'いる': 672, 'うし': -4817, 'うん': 665, 'から': 3472, 'がら': 600, 'こう': -790, 'こと': 2083, 'こん': -1262, 'さら': -4143, 'さん': 4573, 'した':
2641, 'して': 1104, 'すで': -3399, 'そこ': 1977, 'それ': -871, 'たち': 1122, 'ため': 601, 'った': 3463, 'つい': -802, 'てい': 805, 'てき': 1249, 'でき':
1127, 'です': 3445, 'では': 844, 'とい': -4915, 'とみ': 1922, 'どこ': 3887, 'ない': 5713, 'なっ': 3015, 'など': 7379, 'なん': -1113, 'にし': 2468, 'には':
1498, 'にも': 1671, 'に対': -912, 'の一': -501, 'の中': 741, 'ませ': 2448, 'まで': 1711, 'まま': 2600, 'まる': -2155, 'やむ': -1947, 'よっ': -2565, 'れた':
2369, 'れで': -913, 'をし': 1860, 'を見': 731, '亡く': -1886, '京都': 2558, '取り': -2784, '大き': -2604, '大阪': 1497, '平方': -2314, '引き': -1336
, '日本': -195, '本当': -2423, '毎日': -2113, '目指': -724};
  this.BW2__ = {'11': -669, '．．': -11822, '――': -5730, '−−': -13175, 'いう': -1609, 'うか': 2490, 'かし': -1350, 'かも': -602, 'から': -7194
, 'かれ': 4612, 'がい': 853, 'がら': -3198, 'きた': 1941, 'くな': -1597, 'こと': -8392, 'この': -4193, 'させ': 4533, 'され': 13168, 'さん': -3977, 'しい': -
1819, 'しか': -545, 'した': 5078, 'して': 972, 'しな': 939, 'その': -3744, 'たい': -1253, 'たた': -662, 'ただ': -3857, 'たち': -786, 'たと': 1224, 'たは': -
939, 'った': 4589, 'って': 1647, 'っと': -2094, 'てい': 6144, 'てき': 3640, 'てく': 2551, 'ては': -3110, 'ても': -3065, 'でい': 2666, 'でき': -1528, 'でし': -
3828, 'です': -4761, 'でも': -4203, 'とい': 1890, 'とこ': -1746, 'とと': -2279, 'との': 720, 'とみ': 5168, 'とも': -3941, 'ない': -2488, 'なが': -1313
, 'など': -6509, 'なの': 2614, 'なん': 3099, 'にお': -1615, 'にし': 2748, 'にな': 2454, 'によ': -7236, 'に対': -14943, 'に従': -4688, 'に関': -11388
, 'のか': 2093, 'ので': -7059, 'のに': -6041, 'のの': -6125, 'はい': 1073, 'はが': -1033, 'はず': -2532, 'ばれ': 1813, 'まし': -1316, 'まで': -6621, 'まれ':
5409, 'めて': -3153, 'もい': 2230, 'もの': -10713, 'らか': -944, 'らし': -1611, 'らに': -1897, 'りし': 651, 'りま': 1620, 'れた': 4270, 'れて': 849, 'れば':
4114, 'ろう': 6067, 'われ': 7901, 'を通': -11877, 'んだ': 728, 'んな': -4115, '一人': 602, '一方': -1375, '一日': 970, '一部': -1051, '上が': -4479, '会社': -
1116, '出て': 2163, '分の': -7758, '同党': 970, '同日': -913, '大阪': -2471, '委員': -1250, '少な': -1050, '年度': -8669, '年間': -1626, '府県': -2363
, '手権': -1982, '新聞': -4066, '日新': -722, '日本': -7068, '日米': 3372, '曜日': -601, '朝鮮': -2355, '本人': -2697, '東京': -1543, '然と': -1384, '社会': -
1276, '立て': -990, '第に': -1612, '米国': -4268};
  this.BW3__ = {'あた': -2194, 'あり': 719, 'ある': 3846, 'い．': -1185, 'い。': -1185, 'いい': 5308, 'いえ': 2079, 'いく': 3029, 'いた': 2056, 'いっ':
1883, 'いる': 5600, 'いわ': 1527, 'うち': 1117, 'うと': 4798, 'えと': 1454, 'か．': 2857, 'か。': 2857, 'かけ': -743, 'かっ': -4098, 'かに': ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.TokenizerJa.super_"></a>[function <span class="apidocSignatureSpan">natural.TokenizerJa.</span>super_ ()](#apidoc.element.natural.TokenizerJa.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.TokenizerJa.prototype"></a>[module natural.TokenizerJa.prototype](#apidoc.module.natural.TokenizerJa.prototype)

#### <a name="apidoc.element.natural.TokenizerJa.prototype.ctype_"></a>[function <span class="apidocSignatureSpan">natural.TokenizerJa.prototype.</span>ctype_ (str)](#apidoc.element.natural.TokenizerJa.prototype.ctype_)
- description and source-code
```javascript
ctype_ = function (str) {
  for (var i = 0, length = this.chartype_.length; i < length; i++) {
    if (str.match(this.chartype_[i][0])) {
      return this.chartype_[i][1];
    }
  }
  return 'O';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.TokenizerJa.prototype.removePuncTokens"></a>[function <span class="apidocSignatureSpan">natural.TokenizerJa.prototype.</span>removePuncTokens (tokens)](#apidoc.element.natural.TokenizerJa.prototype.removePuncTokens)
- description and source-code
```javascript
removePuncTokens = function (tokens) {
  return tokens
      .map(function(token) {
        return token.replace(/[＿－・，、；：！？．。（）［］｛｝｢｣＠＊＼／＆＃％｀＾＋＜＝＞｜～≪≫─＄＂_\-･,､;:!?.｡()[\]{}「」@*\/&#%'^+<=>|~«»$"\s]+/g, '');
      })
      .filter(function(token) {
        return token != '';
      });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.TokenizerJa.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.TokenizerJa.prototype.</span>tokenize (text)](#apidoc.element.natural.TokenizerJa.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (text) {
  if (text == null || text == undefined || text == '') {
    return [];
  }
  text = normalize(text);
  var result = [];
  var seg = ['B3', 'B2', 'B1'];
  var ctype = ['O', 'O', 'O'];
  var o = text.split('');
  var i;
  var length;
  for (i = 0, length = o.length; i < length; ++i) {
    seg.push(o[i]);
    ctype.push(this.ctype_(o[i]));
  }
  seg.push('E1');
  seg.push('E2');
  seg.push('E3');
  ctype.push('O');
  ctype.push('O');
  ctype.push('O');
  var word = seg[3];
  var p1 = 'U';
  var p2 = 'U';
  var p3 = 'U';
  for (i = 4, length = seg.length - 3; i < length; ++i) {
    var score = this.BIAS__;
    var w1 = seg[i - 3];
    var w2 = seg[i - 2];
    var w3 = seg[i - 1];
    var w4 = seg[i];
    var w5 = seg[i + 1];
    var w6 = seg[i + 2];
    var c1 = ctype[i - 3];
    var c2 = ctype[i - 2];
    var c3 = ctype[i - 1];
    var c4 = ctype[i];
    var c5 = ctype[i + 1];
    var c6 = ctype[i + 2];
    score += this.ts_(this.UP1__[p1]);
    score += this.ts_(this.UP2__[p2]);
    score += this.ts_(this.UP3__[p3]);
    score += this.ts_(this.BP1__[p1 + p2]);
    score += this.ts_(this.BP2__[p2 + p3]);
    score += this.ts_(this.UW1__[w1]);
    score += this.ts_(this.UW2__[w2]);
    score += this.ts_(this.UW3__[w3]);
    score += this.ts_(this.UW4__[w4]);
    score += this.ts_(this.UW5__[w5]);
    score += this.ts_(this.UW6__[w6]);
    score += this.ts_(this.BW1__[w2 + w3]);
    score += this.ts_(this.BW2__[w3 + w4]);
    score += this.ts_(this.BW3__[w4 + w5]);
    score += this.ts_(this.TW1__[w1 + w2 + w3]);
    score += this.ts_(this.TW2__[w2 + w3 + w4]);
    score += this.ts_(this.TW3__[w3 + w4 + w5]);
    score += this.ts_(this.TW4__[w4 + w5 + w6]);
    score += this.ts_(this.UC1__[c1]);
    score += this.ts_(this.UC2__[c2]);
    score += this.ts_(this.UC3__[c3]);
    score += this.ts_(this.UC4__[c4]);
    score += this.ts_(this.UC5__[c5]);
    score += this.ts_(this.UC6__[c6]);
    score += this.ts_(this.BC1__[c2 + c3]);
    score += this.ts_(this.BC2__[c3 + c4]);
    score += this.ts_(this.BC3__[c4 + c5]);
    score += this.ts_(this.TC1__[c1 + c2 + c3]);
    score += this.ts_(this.TC2__[c2 + c3 + c4]);
    score += this.ts_(this.TC3__[c3 + c4 + c5]);
    score += this.ts_(this.TC4__[c4 + c5 + c6]);
    //score += this.ts_(this.TC5__[c4 + c5 + c6]);
    score += this.ts_(this.UQ1__[p1 + c1]);
    score += this.ts_(this.UQ2__[p2 + c2]);
    score += this.ts_(this.UQ3__[p3 + c3]);
    score += this.ts_(this.BQ1__[p2 + c2 + c3]);
    score += this.ts_(this.BQ2__[p2 + c3 + c4]);
    score += this.ts_(this.BQ3__[p3 + c2 + c3]);
    score += this.ts_(this.BQ4__[p3 + c3 + c4]);
    score += this.ts_(this.TQ1__[p2 + c1 + c2 + c3]);
    score += this.ts_(this.TQ2__[p2 + c2 + c3 + c4]);
    score += this.ts_(this.TQ3__[p3 + c1 + c2 + c3]);
    score += this.ts_(this.TQ4__[p3 + c2 + c3 + c4]);
    var p = 'O';
    if (score > 0) {
      result.push(word);
      word = '';
      p = 'B';
    }
    p1 = p2;
    p2 = p3;
    p3 = p;
    word += seg[i];
  }
  result.push(word);

  result = this.removePuncTokens(result);

  return result;
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```

#### <a name="apidoc.element.natural.TokenizerJa.prototype.ts_"></a>[function <span class="apidocSignatureSpan">natural.TokenizerJa.prototype.</span>ts_ (v)](#apidoc.element.natural.TokenizerJa.prototype.ts_)
- description and source-code
```javascript
ts_ = function (v) {
  if (v) { return v; }
  return 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.TreebankWordTokenizer"></a>[module natural.TreebankWordTokenizer](#apidoc.module.natural.TreebankWordTokenizer)

#### <a name="apidoc.element.natural.TreebankWordTokenizer.TreebankWordTokenizer"></a>[function <span class="apidocSignatureSpan">natural.</span>TreebankWordTokenizer ()](#apidoc.element.natural.TreebankWordTokenizer.TreebankWordTokenizer)
- description and source-code
```javascript
TreebankWordTokenizer = function () {
}
```
- example usage
```shell
...
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
console.log(tokenizer.tokenize("my dog hasn't any fleas."));
// [ 'my', 'dog', 'has', 'n\'t', 'any', 'fleas', '.' ]

tokenizer = new natural.RegexpTokenizer({pattern: /\-/});
console.log(tokenizer.tokenize("flea-dog"));
// [ 'flea', 'dog' ]
...
```

#### <a name="apidoc.element.natural.TreebankWordTokenizer.super_"></a>[function <span class="apidocSignatureSpan">natural.TreebankWordTokenizer.</span>super_ ()](#apidoc.element.natural.TreebankWordTokenizer.super_)
- description and source-code
```javascript
super_ = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.TreebankWordTokenizer.prototype"></a>[module natural.TreebankWordTokenizer.prototype](#apidoc.module.natural.TreebankWordTokenizer.prototype)

#### <a name="apidoc.element.natural.TreebankWordTokenizer.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">natural.TreebankWordTokenizer.prototype.</span>tokenize (text)](#apidoc.element.natural.TreebankWordTokenizer.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (text) {
    contractions2.forEach(function(regexp) {
	text = text.replace(regexp,"$1 $2");
    });

    contractions3.forEach(function(regexp) {
	text = text.replace(regexp,"$1 $2 $3");
    });

    // most punctuation
    text = text.replace(/([^\w\.\'\-\/\+\<\>,&])/g, " $1 ");

    // commas if followed by space
    text = text.replace(/(,\s)/g, " $1");

    // single quotes if followed by a space
    text = text.replace(/('\s)/g, " $1");

    // periods before newline or end of string
    text = text.replace(/\. *(\n|$)/g, " . ");

    return  _.without(text.split(/\s+/), '');	
}
```
- example usage
```shell
...

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
tokenizer = new natural.TreebankWordTokenizer();
...
```



# <a name="apidoc.module.natural.Trie"></a>[module natural.Trie](#apidoc.module.natural.Trie)

#### <a name="apidoc.element.natural.Trie.Trie"></a>[function <span class="apidocSignatureSpan">natural.</span>Trie (caseSensitive)](#apidoc.element.natural.Trie.Trie)
- description and source-code
```javascript
function Trie(caseSensitive) {
	this.dictionary = {};
	this.$ = false;

	if(typeof caseSensitive === "undefined") {
		caseSensitive = true;
	}

	this.cs = caseSensitive;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.Trie.prototype"></a>[module natural.Trie.prototype](#apidoc.module.natural.Trie.prototype)

#### <a name="apidoc.element.natural.Trie.prototype.addString"></a>[function <span class="apidocSignatureSpan">natural.Trie.prototype.</span>addString (string)](#apidoc.element.natural.Trie.prototype.addString)
- description and source-code
```javascript
addString = function (string) {
	if(this.cs === false) {
		string = string.toLowerCase();
	}

	// If the string has only one letter, mark this as a word.
	if(string.length === 0) {
		var wasWord = this.$;
		this.$ = true;
		return wasWord;
	}

	// Make sure theres a Trie node in our dictionary
	var next = this.dictionary[string[0]];

	if(!next) {
		this.dictionary[string[0]] = new Trie(this.cs);
		next = this.dictionary[string[0]];
	}

	// Continue adding the string
	return next.addString(string.substring(1));
}
```
- example usage
```shell
...
'''javascript
var natural = require('natural'),
    Trie = natural.Trie;

var trie = new Trie();

// Add one string at a time
trie.addString("test");

// Or add many strings
trie.addStrings(["string1", "string2", "string3"]);
'''

### Searching
...
```

#### <a name="apidoc.element.natural.Trie.prototype.addStrings"></a>[function <span class="apidocSignatureSpan">natural.Trie.prototype.</span>addStrings (list)](#apidoc.element.natural.Trie.prototype.addStrings)
- description and source-code
```javascript
addStrings = function (list) {
	for(var i in list) {
		this.addString(list[i]);
	}
}
```
- example usage
```shell
...

var trie = new Trie();

// Add one string at a time
trie.addString("test");

// Or add many strings
trie.addStrings(["string1", "string2", "string3"]);
'''

### Searching

#### Contains

The most basic operation on a Trie is to see if a search string is marked as a word in the Trie.
...
```

#### <a name="apidoc.element.natural.Trie.prototype.contains"></a>[function <span class="apidocSignatureSpan">natural.Trie.prototype.</span>contains (string)](#apidoc.element.natural.Trie.prototype.contains)
- description and source-code
```javascript
contains = function (string) {
	if(this.cs === false) {
		string = string.toLowerCase();
	}

	if(string.length === 0) {
		return this.$;
	}

	// Otherwise, we need to continue searching
	var firstLetter = string[0];
	var next = this.dictionary[firstLetter];		

	// If we don't have a node, this isn't a word
	if(!next) {
		return false;
	}

	// Otherwise continue the search at the next node
	return next.contains(string.substring(1));
}
```
- example usage
```shell
...
### Searching

#### Contains

The most basic operation on a Trie is to see if a search string is marked as a word in the Trie.

'''javascript
console.log(trie.contains("test")); // true
console.log(trie.contains("asdf")); // false
'''

### Find Prefix

The find prefix search will find the longest prefix that is identified as a word in the trie.
It will also return the remaining portion of the string which it was not able to match.
...
```

#### <a name="apidoc.element.natural.Trie.prototype.findMatchesOnPath"></a>[function <span class="apidocSignatureSpan">natural.Trie.prototype.</span>findMatchesOnPath (search)](#apidoc.element.natural.Trie.prototype.findMatchesOnPath)
- description and source-code
```javascript
findMatchesOnPath = function (search) {
	if(this.cs === false) {
		search = search.toLowerCase();
	}

	function recurse(node, search, stringAgg, resultsAgg) {
		// Check if this is a word.
		if(node.$) {
			resultsAgg.push(stringAgg);
		}

		// Check if the have completed the seearch
		if(search.length === 0) {
			return resultsAgg;
		}

		// Otherwise, continue searching
		var next = node.dictionary[search[0]];
		if(!next) {
			return resultsAgg;
		}
		return recurse(next, search.substring(1), stringAgg + search[0], resultsAgg);
	};

	return recurse(this, search, "", []);
}
```
- example usage
```shell
...
### All Prefixes on Path

This search will return all prefix matches along the search string path.

'''javascript
trie.addString("tes");
trie.addString("est");
console.log(trie.findMatchesOnPath("tester")); // ['tes', 'test'];
'''

### All Keys with Prefix

This search will return all of the words in the Trie with the given prefix, or [ ] if not found.

'''javascript
...
```

#### <a name="apidoc.element.natural.Trie.prototype.findPrefix"></a>[function <span class="apidocSignatureSpan">natural.Trie.prototype.</span>findPrefix (search)](#apidoc.element.natural.Trie.prototype.findPrefix)
- description and source-code
```javascript
findPrefix = function (search) {
	if(this.cs === false) {
		search = search.toLowerCase();
	}
	
	function recurse(node, search, stringAgg, lastWord) {
		// Check if this is a word
		if(node.$) {
			lastWord = stringAgg;
		}

		// Check if we have no more to search
		if(search.length === 0) {
			return [lastWord, search];
		}

		// Continue searching
		var next = node.dictionary[search[0]];
		if(!next) {
			return [lastWord, search];
		}
		return recurse(next, search.substring(1), stringAgg + search[0], lastWord);
	};

	return recurse(this, search, "", null);
}
```
- example usage
```shell
...

### Find Prefix

The find prefix search will find the longest prefix that is identified as a word in the trie.
It will also return the remaining portion of the string which it was not able to match.

'''javascript
console.log(trie.findPrefix("tester"));     // ['test', 'er']
console.log(trie.findPrefix("string4"));    // [null, '4']
console.log(trie.findPrefix("string3"));    // ['string3', '']
'''

### All Prefixes on Path

This search will return all prefix matches along the search string path.
...
```

#### <a name="apidoc.element.natural.Trie.prototype.getSize"></a>[function <span class="apidocSignatureSpan">natural.Trie.prototype.</span>getSize ()](#apidoc.element.natural.Trie.prototype.getSize)
- description and source-code
```javascript
getSize = function () {
	var total = 1;
	for(var c in this.dictionary) {
		total += this.dictionary[c].getSize();
	}
	return total;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.natural.Trie.prototype.keysWithPrefix"></a>[function <span class="apidocSignatureSpan">natural.Trie.prototype.</span>keysWithPrefix (prefix)](#apidoc.element.natural.Trie.prototype.keysWithPrefix)
- description and source-code
```javascript
keysWithPrefix = function (prefix) {
    if(this.caseSensitive === false) {
        prefix = prefix.toLowerCase();
    }

    function isEmpty (object) {
        for (var key in object) if (object.hasOwnProperty(key)) return false;
        return true;
    }

    function get (node, word) {
        if(!node) return null;
        if(word.length == 0) return node;
        return get(node.dictionary[word[0]], word.substring(1));
    }

    function recurse ( node, stringAgg, resultsAgg) {
        if (!node) return;

        // Check if this is a word
        if (node.$) {
            resultsAgg.push(stringAgg);
        }

        if (isEmpty(node.dictionary)) {
            return ;
        }

        for (var c in node.dictionary) {
            recurse (node.dictionary[c],stringAgg + c, resultsAgg);
        }
    }

    var results = [];
    recurse (get(this, prefix), prefix, results);
    return results;
}
```
- example usage
```shell
...
'''

### All Keys with Prefix

This search will return all of the words in the Trie with the given prefix, or [ ] if not found.

'''javascript
console.log(trie.keysWithPrefix("string")); // ["string1", "string2", "string3"]
'''

### Case-Sensitivity

By default the trie is case-sensitive, you can use it in case-_in_sensitive mode by passing 'false'
to the Trie constructor.
...
```



# <a name="apidoc.module.natural.WordPunctTokenizer"></a>[module natural.WordPunctTokenizer](#apidoc.module.natural.WordPunctTokenizer)

#### <a name="apidoc.element.natural.WordPunctTokenizer.WordPunctTokenizer"></a>[function <span class="apidocSignatureSpan">natural.</span>WordPunctTokenizer (options)](#apidoc.element.natural.WordPunctTokenizer.WordPunctTokenizer)
- description and source-code
```javascript
WordPunctTokenizer = function (options) {
    this._pattern = new RegExp(/(\w+|[а-я0-9_]+|\.|\!|\'|\"")/i);
    RegexpTokenizer.call(this,options)
}
```
- example usage
```shell
...
console.log(tokenizer.tokenize("my dog hasn't any fleas."));
// [ 'my', 'dog', 'has', 'n\'t', 'any', 'fleas', '.' ]

tokenizer = new natural.RegexpTokenizer({pattern: /\-/});
console.log(tokenizer.tokenize("flea-dog"));
// [ 'flea', 'dog' ]

tokenizer = new natural.WordPunctTokenizer();
console.log(tokenizer.tokenize("my dog hasn't any fleas."));
// [ 'my',  'dog',  'hasn',  '\'',  't',  'any',  'fleas',  '.' ]
'''

## String Distance

Natural provides an implementation of the [Jaro–Winkler](http://en.wikipedia.org/wiki/Jaro%E2%80%93Winkler_distance) string distance
 measuring algorithm.
...
```

#### <a name="apidoc.element.natural.WordPunctTokenizer.super_"></a>[function <span class="apidocSignatureSpan">natural.WordPunctTokenizer.</span>super_ (options)](#apidoc.element.natural.WordPunctTokenizer.super_)
- description and source-code
```javascript
super_ = function (options) {
    var options = options || {};
    this._pattern = options.pattern || this._pattern;
    this.discardEmpty = options.discardEmpty || true;

    // Match and split on GAPS not the actual WORDS
    this._gaps = options.gaps;

    if (this._gaps === undefined) {
        this._gaps = true;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.natural.WordTokenizer"></a>[module natural.WordTokenizer](#apidoc.module.natural.WordTokenizer)

#### <a name="apidoc.element.natural.WordTokenizer.WordTokenizer"></a>[function <span class="apidocSignatureSpan">natural.</span>WordTokenizer (options)](#apidoc.element.natural.WordTokenizer.WordTokenizer)
- description and source-code
```javascript
WordTokenizer = function (options) {
    this._pattern = /[^A-Za-zА-Яа-я0-9_]+/;
    RegexpTokenizer.call(this,options)
}
```
- example usage
```shell
...
## Tokenizers

Word, Regexp, and [Treebank tokenizers](http://www.cis.upenn.edu/~treebank/tokenization.html) are provided for breaking text up
into
arrays of tokens:

'''javascript
var natural = require('natural'),
  tokenizer = new natural.WordTokenizer();
console.log(tokenizer.tokenize("your dog has fleas."));
// [ 'your', 'dog', 'has', 'fleas' ]
'''

The other tokenizers follow a similar pattern:

'''javascript
...
```

#### <a name="apidoc.element.natural.WordTokenizer.super_"></a>[function <span class="apidocSignatureSpan">natural.WordTokenizer.</span>super_ (options)](#apidoc.element.natural.WordTokenizer.super_)
- description and source-code
```javascript
super_ = function (options) {
    var options = options || {};
    this._pattern = options.pattern || this._pattern;
    this.discardEmpty = options.discardEmpty || true;

    // Match and split on GAPS not the actual WORDS
    this._gaps = options.gaps;

    if (this._gaps === undefined) {
        this._gaps = true;
    }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
