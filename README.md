# Awesome NLP Resources for Hungarian [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/oroszgy/awesome-hungarian-nlp)

> A curated list of *free* resources dedicated to Hungarian Natural Language Processing
>
> Maintainers - [György Orosz](https://github.com/oroszgy)

## Table of contents

1. [Tools](#1-tools)
2. [Datasets](#2-datasets)
3. [Journals / Conferences / Institutes / Events](#3-journals--conferences--institutes--events)
4. [Courses / Tutorials](#4-courses--tutorials)
5. [Blogs / Communities](#5-blogs--communities)

## 1. Tools

Notations:

- 👌 Easy to install and use
- 🚀 Commercial-friendly license
- 💯 Pretrained models are available or not needed

### Word tokenization, sentence splitting

- [huntoken](https://github.com/zseder/huntoken) 👌🚀💯 Hungarian word and sentence splitter
- [quntoken](https://github.com/dlt-rilmta/quntoken) 👌🚀💯 New Hungarian tokenizer based on quex, huntoken

### Morphology

- [emMorph (Humor)](https://github.com/dlt-rilmta/emMorph) 💯 Hungarian morphological analyzer based on Humor
- [emMorphPy](https://github.com/ppke-nlpg/emmorphpy) 👌💯A wrapper, a lemmatizer and REST API implemented in Python for emMorph (Humor) Hungarian morphological analyzer
- [hunmorph](http://mokk.bme.hu/resources/hunmorph/) 🚀💯 is an open source tool and programming library for spell-checking, stemming and morphological analysing of agglutinative, german and other languages.
- [hunmorph-foma](https://github.com/r0ller/hunmorph-foma) 🚀💯 Hungarian morpholical analyzer and generator based on hunmorph.
- [hunspell](http://hunspell.github.io/) 👌🚀💯 is an open-source spell-checker, stemmer and morphological analyzer
- [lara-hungarian-nlp](https://github.com/sedthh/lara-hungarian-nlp) 👌🚀💯 LARA is a lightweight Python NLP library for ChatBots in Hungarian.
- [Lemmagen](http://lemmatise.ijs.si/) 👌🚀💯 project aims at providing standardized open source multilingual platform for lemmatisation. ([Python package for v2](https://pypi.python.org/pypi/Lemmagen) | [C# project for v3](https://github.com/oroszgy/lemmagen3))

### PoS / Morphological taggers

- [hunpos](http://mokk.bme.hu/resources/hunpos/) 👌🚀💯 Hunpos is an open source reimplementation of TnT, the well known part-of-speech tagger by Thorsten Brants.
- [PurePos](https://github.com/ppke-nlpg/purepos) 👌🚀 Open source morphological tagger based on HunPos
- [purepos.py](https://github.com/ppke-nlpg/purepos.py) 👌🚀 Python wrapper for PurePos

### Taggers / Chunkers

- [HunTag](https://github.com/recski/HunTag) 👌🚀 A sequential tagger for NLP using Maximum Entropy Learning and Hidden Markov Models
- [HunTag3](https://github.com/ppke-nlpg/HunTag3) 👌🚀 Improved version of the original HunTag
- [SzegedNER](http://rgai.inf.u-szeged.hu/NER) 👌🚀💯 Named Entity Recognition tool for Hungarian and English
- [DBpedia Spotlight](https://github.com/dbpedia-spotlight/dbpedia-spotlight) 👌🚀💯  DBpedia Spotlight is a tool for automatically annotating mentions of DBpedia resources in text. [Docker image](https://hub.docker.com/r/dbpedia/spotlight-hungarian/)

### Pipelines with Hungarian NLP components

- [magyarlanc](http://rgai.inf.u-szeged.hu/magyarlanc) 👌💯 A toolkit for the basic linguistic processing of Hungarian
- [magyarlanc_spark](https://github.com/tyson925/
lanc_spark) 👌💯 Spark wrapper for magyarlanc
- [spaCy](https://github.com/explosion/spaCy) 👌🚀💯 Industrial-strength Natural Language Processing (NLP) with Python and Cython ([Hungarian models](https://github.com/oroszgy/spacy-hungarian-models))
- [huNLP](https://github.com/oroszgy/hunlp) 👌💯 Unified Java and REST API for magyarlanc and szegedNER
- [hunlp-GATE](https://github.com/dlt-rilmta/hunlp-GATE) 💯 GATE plugin containing Hungarian NLP tools as GATE processing resources
- [Trendminer Hungarian Processing Pipeline](https://github.com/mmihaltz/trendminer-hunlp) 🚀 Hungarian NLP pipeline for social media text analysis (TrendMiner project)
- [Google Syntaxnet](https://research.googleblog.com/2017/03/an-upgrade-to-syntaxnet-new-models-and.html) 🚀💯 Neural Models of Syntax
- [UDPipe](http://ufal.mff.cuni.cz/udpipe) 👌🚀💯 is a trainable pipeline for tokenization, tagging, lemmatization and dependency parsing of CoNLL-U files
- [polyglot](http://polyglot.readthedocs.io/en/latest/index.html) 👌🚀💯 is a natural language pipeline that supports massive multilingual applications.
- [emtsv](https://github.com/dlt-rilmta/emtsv) 👌💯 is a text processing system with inter-module communication via tsv + REST API

### Syntactic parsers

- [hunpars](http://mokk.bme.hu/resources/hunpars/) 🚀💯 A rule based Hungarian syntactical analyzer
- [HunParse](https://github.com/recski/HunParse) 🚀💯 An NLTK-based parser using KR-style morphological annotation
- [Anagramma Parser](https://github.com/ppke-nlpg/AnaGramma-Parser) A parser based on psycholinguistics principles

### Semantic analysis

- [SentimentAnalysisHUN](https://github.com/dhuszti/SentimentAnalysisHUN) 👌🚀💯 is an open-source sentiment analysis tool for Hungarian language, written in Python.

### Other

- [emLam](https://github.com/dlt-rilmta/emLam) 👌🚀💯 Preprocessing scripts for Hungarian Language Modeling
- [pywnxml](https://github.com/ppke-nlpg/pywnxml) 👌🚀💯 Python3 API for WordNet XML (Hungarian WordNet / BalkaNet / VisDic format)

## 2. Datasets

### Corpora

- [Hungarian Webcorpus](http://mokk.bme.hu/resources/webcorpus/) With over 1.48 billion words unfiltered (589m words fully filtered), this is by far the largest Hungarian language corpus, and unlike the Hungarian National Corpus (125m words), it is available in its entirety under a permissive Open Content license.
- [emLam](https://hlt.bme.hu/en/resources/emLam) A Language Modeling Benchmark Corpus for Hungarian, similar to the One Billion Word corpus (Chelba, 2014) for English.
- [Leipzig corpora](http://wortschatz.uni-leipzig.de/en/download/) contains randomly selected sentences in the language of the corpus and are available in sizes from 10,000 sentences up to 1 million sentences. The sources are either newspaper texts or texts randomly collected from the web.
- [web2corpus](http://ufal.mff.cuni.cz/w2c) Automatically create multilingual web corpus
- [CoNLL 2017: Automatically Annotated Raw Texts and Word Embeddings](https://lindat.mff.cuni.cz/repository/xmlui/handle/11234/1-1989) Automatic segmentation, tokenization and morphological and syntactic annotations of raw texts in 45 languages, generated by [UDPipe](http://ufal.mff.cuni.cz/udpipe), together with word embeddings of dimension 100 computed from lowercased texts by [word2vec](https://code.google.com/archive/p/word2vec/)
- [OpinHuBank](https://sites.google.com/site/mmihaltz/resources) OpinHuBank is a human-annotated corpus to aid the research of opinion mining and sentiment analysis in Hungarian
- [The Hungarian forum corpus for Opinion Mining](http://rgai.inf.u-szeged.hu/index.php?lang=en&page=corpus_forum) This database is the first one dedicated to Opinion Mining in Hungarian. The data for further processing were gathered from the posts of the forum topic of the Hungarian government portal dealing with the referendum about dual citizenship.
- [Szeged Treebank](http://rgai.inf.u-szeged.hu/index.php?lang=en&page=SzegedTreebank) The Szeged Treebank is the largest fully manually annotated treebank of the Hungarian language
- [Szeged Dependency Treebank](http://rgai.inf.u-szeged.hu/index.php?lang=en&page=dependency) The Szeged Dependency Treebank is a dependency-tree format version of the Szeged Treebank.
- [Universal Dependencies](https://github.com/UniversalDependencies/UD_Hungarian)
- [Hungarian Named Entity Corpora](http://rgai.inf.u-szeged.hu/index.php?lang=en&page=corpus_ne) The Named Entity Corpus for Hungarian is a subcorpus of the Szeged Treebank, which contains full syntactic annotations done manually by linguist experts.
- [hunNERwiki](http://hlt.sztaki.hu/resources/hunnerwiki.html) a silver standard corpus for Hungarian Named Entity Recognition
- [Mazsola database](http://corpus.nytud.hu/isz/) containes 28M sentences from the MNSZ1 corpus annotated with shallow syntactic analysis 
- [Hungarian word sense disambiguated corpus](http://rgai.inf.u-szeged.hu/index.php?lang=en&page=corpus_hunwsd) containing 39 suitable word form samples for the purpose of word sense disambiguation
- [HunLearner](http://rgai.inf.u-szeged.hu/index.php?lang=en&page=hunlearner) is a learners' corpus of Hungarian containing written data from 35 students majoring in Hungarian studies at the University of Zagreb, Croatia. Texts were morphologically and syntactically analyzed by the magyarlanc tool.
- [Hunglish Corpus](http://mokk.bme.hu/resources/hunglishcorpus/) The Hunglish Corpus is a free sentence-aligned Hungarian-English parallel corpus of about 120 million words in 4 million sentence pairs. 
- [SzegedParallel](http://rgai.inf.u-szeged.hu/index.php?lang=en&page=corpus_paralell) The English-Hungarian parallel corpus contains texts selected on the basis of grammatical and translational criteria.
- [HunOr](http://rgai.inf.u-szeged.hu/index.php?lang=en&page=corpus_hunor) A Hungarian-Russian Parallel corpus comprises approximately 800 thousand words.
- [CoNLL 2017 Shared Task Hungarian data](https://lindat.mff.cuni.cz/repository/xmlui/handle/11234/1-1989) Automatic segmentation, tokenization and morphological and syntactic annotations of raw texts from the Common Crawl
- [CSS10](https://github.com/Kyubyong/css10) A Collection of Single Speaker Speech Datasets for 10 Languages including Hungarian

### Word vectors

- [FasText Wikipedia](https://github.com/facebookresearch/fastText/blob/master/pretrained-vectors.md) pre-trained word vectors for 90 languages, trained on Wikipedia using fastText.
- [FastText_multilingual](https://github.com/Babylonpartners/fastText_multilingual) Multilingual word vectors in 78 languages
- [polyglot vectors](https://sites.google.com/site/rmyeid/projects/polyglot) polgyglot embeddings on Wikipedia
- [wordvectors](https://github.com/Kyubyong/wordvectors) Pre-trained word2vec and fasttext word vectors on wikipedia of 30+ languages
- [hunembed0.0](http://corpus.nytud.hu/efnilex-vect/) A word2vec word embedding trained on the concatenation of the Hungarian Webcorpus and the Hungarian National Corpus in 600 dimensions with a cut-off of 10 words.
- [Szeged word vectors](http://rgai.inf.u-szeged.hu/project/nlp/research/w2v/doc.html) Word embeddings (word2vec & fasttext) for Hungarian trained on 4.3 billion tokens
- [questions-words-hu](http://corpus.nytud.hu/efnilex-vect/data/questions-words-hu.txt) Hungarian analogical questions following Mikolov et al. 
- [Conceptnet Numberbatch](https://github.com/commonsense/conceptnet-numberbatch) Conceptnet numbermatch multi- and cross-lingual semantic word embeddings
- [Multi-sense word embeddings](https://hlt.bme.hu/en/publ/makrai17)
- [ELMo Representations](https://github.com/HIT-SCIR/ELMoForManyLangs) Deep contextualized word representation trained for many languages

### Linguistic Resources

- [morphdb.hu](http://mokk.bme.hu/resources/morphdb-hu/) is an open source morphological database of Hungarian, consisting of a lexicon and morphological grammar that are based on well-founded theoretical decisions.
- [huwn](https://github.com/mmihaltz/huwn) Hungarian Wordnet
- [Hungarian Sentiment Lexicon](http://opendata.hu/dataset/hungarian-sentiment-lexicon) The dictionaries were manually created on the basis of Wordnet-Affect lexicons.
- [4lang](https://github.com/kornai/4lang) Concept dictionary using Eilenberg machines
- [Named Entity lists for Hungarian](http://rgai.inf.u-szeged.hu/project/nlp/download/corpora/NER_dictionaries.zip)
- [Mazsola ISZ](http://corpus.nytud.hu/isz/) lists 500K verb frames extracted from the Mazsola database
- [Manocska](https://github.com/ppke-nlpg/manocska) merges verb frames existing databases

### Linked Open Data

- [Wikipedia dumps](https://dumps.wikimedia.org/huwiki/)
- [DBPedia dumps](http://downloads.dbpedia.org/current/core-i18n/hu/)
- [huwn.rdf](https://github.com/mmihaltz/huwn.rdf) Hungarian WordNet in RDF format for the Linked Open Data cloud

## 3. Journals / Conferences / Institutes / Events

### Journals

- [Acta Cybernetica](https://www.inf.u-szeged.hu/kutatas/acta-cybernetica)

### Conferences

- MSZNY (Conference on Hungarian Computational Linguistics) [2018](http://rgai.inf.u-szeged.hu/index.php?lang=hu&page=mszny2018) [2017](http://rgai.inf.u-szeged.hu/index.php?lang=hu&page=mszny2017) [2016](http://rgai.inf.u-szeged.hu/mszny2016/) [2015](http://rgai.inf.u-szeged.hu/mszny2015/) [2014](http://rgai.inf.u-szeged.hu/mszny2014/) [2013](http://www.inf.u-szeged.hu/projectdirs/mszny2013/) [2011](http://www.inf.u-szeged.hu/projectdirs/mszny2011/) [2010](http://www.inf.u-szeged.hu/projectdirs/mszny2010/) [2009](http://www.inf.u-szeged.hu/projectdirs/mszny2009/)

### Institutes

- [Natural Language Processing Group of the Pázmány Péter Catholic University Faculty of Information Tehnology and Bionics](http://nlpg.itk.ppke.hu/)
- [Department of Language Technology and Applied Linguistics, RIL-MTA](http://www.nytud.hu/depts/delts/index.html)
- [Human Language Technology Research Group of the Budapest University of Technology and Economics](http://hlt.bme.hu/en/)
- [Natural Language Processing Group of the Szeged University](http://www.inf.u-szeged.hu/rgai/nlp)
- [BME - Laboratory of Speech Acoustics](http://alpha.tmit.bme.hu/speech/)

## 4. Courses / Tutorials

TBD

- [Tutorial on Text Mining for Hungarian](https://github.com/oroszgy/hungarian-text-mining-workshop)

## 5. Blogs / Communities

- [Kereső világ](http://kereses.blog.hu/) Official blog of Precognox Inc.
- [Hungarian NLP Meetup](https://www.meetup.com/Hungarian-nlp/)
- [Deep Learning Reading Seminar Meetup](https://www.meetup.com/Budapest-Deep-Learning-Reading-Seminar/)
