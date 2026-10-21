# Awesome NLP Resources for Hungarian

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/oroszgy/awesome-hungarian-nlp)
[![Check Links](https://github.com/oroszgy/awesome-hungarian-nlp/actions/workflows/links.yml/badge.svg)](https://github.com/oroszgy/awesome-hungarian-nlp/actions/workflows/links.yml)
[![stars](https://img.shields.io/github/stars/oroszgy/awesome-hungarian-nlp?style=social)](https://github.com/oroszgy/awesome-hungarian-nlp)

> A curated list of *free* resources dedicated to Hungarian Natural Language Processing
>
> Maintainers - [György Orosz](https://github.com/oroszgy)

## Table of contents

<!-- MarkdownTOC autolink="true" markdown_preview="github" style="ordered" indent="   " -->

1. [Tools](#tools)
   1. [Word tokenization, sentence splitting](#word-tokenization-sentence-splitting)
   1. [Morphology](#morphology)
   1. [PoS / Morphological taggers](#pos--morphological-taggers)
   1. [Taggers / Chunkers](#taggers--chunkers)
   1. [Pipelines with Hungarian NLP components](#pipelines-with-hungarian-nlp-components)
   1. [Syntactic parsers](#syntactic-parsers)
   1. [Semantic analysis](#semantic-analysis)
   1. [Machine translation](#machine-translation)
   1. [Summarization](#summarization)
   1. [Classification and extraction](#classification-and-extraction)
   1. [OCR](#ocr)
   1. [Other](#other)
1. [Language models](#language-models)
   1. [Word embeddings](#word-embeddings)
   1. [Transformer models](#transformer-models)
   1. [Speech models](#speech-models)
   1. [Large language models](#large-language-models)
      1. [General multilingual large language models](#general-multilingual-large-language-models)
      1. [Large language models developed for Hungarian use cases](#large-language-models-developed-for-hungarian-use-cases)
   1. [LLM Benchmarks](#llm-benchmarks)
1. [Datasets](#datasets)
   1. [Corpora](#corpora)
      1. [Raw corpora](#raw-corpora)
      1. [Annotated corpora](#annotated-corpora)
      1. [Parallel corpora](#parallel-corpora)
   1. [Linguistic resources](#linguistic-resources)
   1. [Linked Open Data](#linked-open-data)
   1. [Geo data](#geo-data)
   1. [Speech related data](#speech-related-data)
   1. [Other](#other-1)
1. [Academy](#academy)
   1. [Journals](#journals)
   1. [Conferences](#conferences)
   1. [Institutes](#institutes)
1. [Learning resources](#learning-resources)
   1. [Books](#books)
   1. [Courses](#courses)
   1. [Tutorials](#tutorials)
1. [Communities](#communities)
1. [Other Hungarian related resource collections](#other-hungarian-related-resource-collections)

<!-- /MarkdownTOC -->

## Tools

Notations:

- 👌 Easy to install and use
- 🚀 Commercial-friendly license
- 💯 Pretrained models are available or not needed
- 🏛️ Historical: unmaintained or superseded, kept for reference

Sections are split by artifact type: **Tools** are task-specific systems you can run, including fine-tuned models; **Language models** are base and foundation models; **Datasets** are data. Install and licence badges are assessed for Tools entries only.

### Word tokenization, sentence splitting

- [huntoken](https://github.com/zseder/huntoken) 👌🚀💯🏛️ Hungarian word and sentence splitter
- [quntoken](https://github.com/dlt-rilmta/quntoken) 👌🚀💯 New Hungarian tokenizer based on quex, huntoken

### Morphology

- [emMorph (Humor)](https://github.com/dlt-rilmta/emMorph) 💯 Hungarian morphological analyzer based on Humor
- [emMorphPy](https://github.com/ppke-nlpg/emmorphpy) 👌💯 A wrapper, a lemmatizer and REST API implemented in Python for emMorph (Humor) Hungarian morphological analyzer
- [hunmorph](http://mokk.bme.hu/resources/hunmorph/) 🚀💯 is an open source tool and programming library for spell-checking, stemming and morphological analysing of agglutinative, german and other languages.
- [hunmorph-foma](https://github.com/r0ller/hunmorph-foma) 🚀💯 Hungarian morphological analyzer and generator based on hunmorph.
- [hunspell](https://hunspell.github.io/) 👌🚀💯 is an open-source spell-checker, stemmer and morphological analyzer
- [Lemmagen](https://kt.ijs.si/software/lemmagen/) 👌🚀💯 project aims at providing standardized open source multilingual platform for lemmatisation. ([Python package for v3](https://pypi.org/project/lemmagen3/) | [C# project for v3](https://github.com/oroszgy/lemmagen3))
- [Simplemma](https://github.com/adbar/simplemma) 👌🚀💯 is a simple multilingual lemmatizer for Python
- [SampoNLP](https://github.com/AragonerUA/SampoNLP) 👌🚀💯 Unsupervised morpheme discovery for Uralic languages including Hungarian, with a Rust core

### PoS / Morphological taggers

- [hunpos](http://mokk.bme.hu/resources/hunpos/) 👌🚀💯 Hunpos is an open source reimplementation of TnT, the well known part-of-speech tagger by Thorsten Brants.
- [PurePos](https://github.com/ppke-nlpg/purepos) 👌🚀 Open source morphological tagger based on HunPos
- [purepos.py](https://github.com/ppke-nlpg/purepos.py) 👌🚀 Python wrapper for PurePos

### Taggers / Chunkers

- [HunTag](https://github.com/recski/HunTag) 👌🚀 A sequential tagger for NLP using Maximum Entropy Learning and Hidden Markov Models
- [HunTag3](https://github.com/ppke-nlpg/HunTag3) 👌🚀 Improved version of the original HunTag
- [SzegedNER](https://rgai.inf.u-szeged.hu/node/109) 👌🚀💯 Named Entity Recognition tool for Hungarian and English
- [DBpedia Spotlight](https://github.com/dbpedia-spotlight/dbpedia-spotlight) 👌🚀💯  DBpedia Spotlight is a tool for automatically annotating mentions of DBpedia resources in text. [Docker image](https://hub.docker.com/r/dbpedia/dbpedia-spotlight)
- [emBERT](https://github.com/DavidNemeskey/emBERT) 👌🚀💯 is an emtsv module for pre-trained Transformer-based models. It provides tagging models based on Huggingface's transformers package.

### Pipelines with Hungarian NLP components

- [magyarlanc](https://rgai.inf.u-szeged.hu/magyarlanc) 👌💯 A toolkit for the basic linguistic processing of Hungarian
- [magyarlanc_spark](https://github.com/tyson925/magyarlanc_spark) 👌💯🏛️ Spark wrapper for magyarlanc
- [eszterland](https://github.com/damesek/eszterlanc) 👌💯 Clojurized access to magyarlanc
- [HuSpaCy](https://github.com/huspacy/huspacy) 👌🚀💯 Industrial-strength Hungarian Natural Language Processing
- [huNLP](https://github.com/oroszgy/hunlp) 👌💯 An experimental unified Java and REST API for magyarlanc and szegedNER
- [hunlp-GATE](https://github.com/dlt-rilmta/hunlp-GATE) 💯 GATE plugin containing Hungarian NLP tools as GATE processing resources
- [Trendminer Hungarian Processing Pipeline](https://github.com/mmihaltz/trendminer-hunlp) 🚀 Hungarian NLP pipeline for social media text analysis (TrendMiner project)
- [Google Syntaxnet](https://research.googleblog.com/2017/03/an-upgrade-to-syntaxnet-new-models-and.html) 🚀💯🏛️ Neural Models of Syntax
- [UDPipe](https://ufal.mff.cuni.cz/udpipe) 👌🚀💯 is a trainable pipeline for tokenization, tagging, lemmatization and dependency parsing of CoNLL-U files
- [polyglot](https://polyglot.readthedocs.io/en/latest/index.html) 👌🚀💯🏛️ is a natural language pipeline that supports massive multilingual applications.
- [emtsv](https://github.com/dlt-rilmta/emtsv) 👌💯 is a text processing system with inter-module communication via tsv + REST API
- [Stanza](https://github.com/stanfordnlp/stanza) 👌🚀💯 is a Python NLP Library for Many Human Languages
- [trankit](https://github.com/nlp-uoregon/trankit) 👌🚀💯 A Light-Weight Transformer-based Python Toolkit for Multilingual Natural Language Processing

### Syntactic parsers

- [hunpars](http://mokk.bme.hu/resources/hunpars/) 🚀💯 A rule based Hungarian syntactical analyzer
- [HunParse](https://github.com/recski/HunParse) 🚀💯🏛️ An NLTK-based parser using KR-style morphological annotation
- [Anagramma Parser](https://github.com/ppke-nlpg/AnaGramma-Parser) A parser based on psycholinguistics principles
- [benepar](https://github.com/nikitakit/self-attentive-parser) 👌🚀💯🏛️ A high-accuracy parser with models for 11 languages, implemented in Python. Based on Constituency Parsing with a Self-Attentive Encoder from ACL 2018.

### Semantic analysis

- [SentimentAnalysisHUN](https://github.com/dhuszti/SentimentAnalysisHUN) 👌🚀💯🏛️ is an open-source sentiment analysis tool for Hungarian language, written in Python.
- [hun-date-parser](https://github.com/szegedai/hun-date-parser) 👌🚀💯 A tool for extracting datetime intervals from Hungarian sentences and turning datetime objects into Hungarian text.
- [Babel Machine](https://babelmachine.org/) poltextLAB's multilingual policy-topic, emotion and NER classification platform, with the [codebase](https://huggingface.co/poltextlab/babel-machine) available on request

### Machine translation

- [NYTK MT](https://github.com/nytud/machine-translation) 👌🚀💯 NYTK Machine translation models
- [syntax-augmentation-nmt](https://github.com/attilanagy234/syntax-augmentation-nmt) 🚀💯 Syntax-based data augmentation for Hungarian-English machine translation

### Summarization

- SZTAKI HunSum-1 models 👌🚀💯 [mT5-small-HunSum-1](https://huggingface.co/SZTAKI-HLT/mT5-small-HunSum-1), [mT5-base-HunSum-1](https://huggingface.co/SZTAKI-HLT/mT5-base-HunSum-1), [Bert2Bert-HunSum-1](https://huggingface.co/SZTAKI-HLT/Bert2Bert-HunSum-1)
- SZTAKI HunSum-2 models 👌🚀💯 [mT5-base-HunSum-2](https://huggingface.co/SZTAKI-HLT/mT5-base-HunSum-2), [Bert2Bert-HunSum-2](https://huggingface.co/SZTAKI-HLT/Bert2Bert-HunSum-2)

### Classification and extraction

- [kmdb NER](https://huggingface.co/K-Monitor/kmdb_ner_v5) 👌🚀💯 Hungarian NER for people, organisations and places in news, separating entities relevant to the article's case from mere mentions
- [ModernBERT POS](https://huggingface.co/GaborMadarasz/ModernBERT-base-hungarian-POS) 👌🚀💯 Hungarian part-of-speech tagger for long texts (8K context)
- [HuAMR](https://github.com/botondbarta/HuAMR) 👌💯 A Hungarian Abstract Meaning Representation dataset and a suite of LLM-based AMR parsers
- [poltextLAB's models](https://huggingface.co/collections/poltextlab/emotions-babel-672b54c08540c5e11ecb9983) emotion classification models using 6-label and 9-label codebooks.
- [kmdb news classifier](https://huggingface.co/K-Monitor/kmdb_classification_hubert_v5) 👌🚀💯 Decides whether a Hungarian news article reports a corruption, public-spending or transparency case
- [toxic-hubert](https://huggingface.co/RabidUmarell/toxic-hubert) 👌💯 Hungarian toxicity and hate-speech classifier fine-tuned from huBERT (AGPL-3.0)

### OCR

- [ocr-T5](https://huggingface.co/GaborMadarasz/ocr-T5) 👌🚀💯 Hungarian post-OCR correction model based on mT5-large
- [PP-OCRv6 Hungarian antiqua](https://huggingface.co/GaborMadarasz/paddleocr-ppocr6-mek-finetuned) 👌🚀💯 OCR model for 1880–1930 Hungarian antiqua typography, tuned for ő and ű

### Other

- [emLam](https://github.com/dlt-rilmta/emLam) 👌🚀💯 Preprocessing scripts for Hungarian Language Modeling
- [pywnxml](https://github.com/ppke-nlpg/pywnxml) 👌🚀💯 Python3 API for WordNet XML (Hungarian WordNet / BalkaNet / VisDic format)
- [Hun-appointment-chatbot](https://github.com/szegedai/hun-appointment-chatbot) 👌🚀💯 A simple Hungarian chatbot for booking an appointment using the Rasa framework.
- [neural-punctuator](https://github.com/attilanagy234/neural-punctuator) 👌🚀💯 Automatic punctuation restoration with BERT models for English and Hungarian
- [hunaccent](https://github.com/juditacs/hunaccent) 👌🚀💯 Small Footprint Diacritic Restoration for Hungarian
- [Diacritics_restoration](https://github.com/aielte-research/Diacritics_restoration) 🚀💯 Lightweight Diacritics Restoration with Dilated Convolutional Neural Networks
- [anonymizer_hu](https://github.com/nytud/anonymizer_hu) 🚀💯 The Hungarian anonymization tool for CURLICAT
- [WebArticleCurator](https://github.com/ELTE-DH/WebArticleCurator) 👌🚀💯 News article text extraction and boilerplate removal (LGPL-3.0)
- [Kalliopé](https://github.com/aporkolab/Kalliope) 👌🚀💯 Hungarian verse scansion, metre and rhyme-scheme analyzer with web demo, Docker image and REST API
- [lara-hungarian-nlp](https://github.com/sedthh/lara-hungarian-nlp) 👌🚀💯 LARA is a lightweight Python NLP library for ChatBots in Hungarian.

## Language models

### Word embeddings

- [fastText Wikipedia](https://fasttext.cc/docs/en/pretrained-vectors.html) pre-trained word vectors for 90 languages, trained on Wikipedia using fastText.
- [fastText Common Crawl & Wikipedia](https://fasttext.cc/docs/en/crawl-vectors.html) pre-trained word vectors for 157 languages, trained on Wikipedia and the Common Crawl using fastText's CBOW model.
- [FastText_multilingual](https://github.com/Babylonpartners/fastText_multilingual) Multilingual word vectors in 78 languages
- [polyglot vectors](https://sites.google.com/site/rmyeid/projects/polyglot) polyglot embeddings on Wikipedia
- [wordvectors](https://github.com/Kyubyong/wordvectors) Pre-trained word2vec and fasttext word vectors on wikipedia of 30+ languages 🏛️
- [hunembed0.0](http://corpus.nytud.hu/efnilex-vect/) A word2vec word embedding trained on the concatenation of the Hungarian Webcorpus and the Hungarian National Corpus in 600 dimensions with a cut-off of 10 words.
- [Szeged word vectors](https://www.inf.u-szeged.hu/~szantozs/fasttext/) Word embeddings (word2vec & fasttext) for Hungarian trained on 4.3 billion tokens
- [Conceptnet Numberbatch](https://github.com/commonsense/conceptnet-numberbatch) Conceptnet numberbatch multi- and cross-lingual semantic word embeddings
- [Multi-sense word embeddings](https://hlt.bme.hu/en/publ/makrai17)
- [BytePair Embeddings](https://github.com/bheinzerling/bpemb) pretrained subword embeddings, including Hungarian, downloadable in many formats
- [HuSpaCy 300d](https://huggingface.co/huspacy/hu_vectors_web_lg) 300d Floret embeddings trained on the Hungarian Webcorpus 2.0
- [HuSpaCy 100d](https://huggingface.co/huspacy/hu_vectors_web_md) 100d Floret embeddings trained on the Hungarian Webcorpus 2.0
- [ELMo Representations](https://github.com/HIT-SCIR/ELMoForManyLangs) Deep contextualized word representation trained for many languages 🏛️

### Transformer models

- [`huBERT`](https://hlt.bme.hu/en/resources/hubert) Hungarian BERT base models trained on Webcorpus 2.0 and the Hungarian Wikipedia
- [HIL* Transformer models](https://hilanco.github.io) Pretrained transformer models provided by HILANCO
- [PULI-BERT-Large](https://huggingface.co/NYTK/PULI-BERT-Large) is a Hungarian BERT large model based on MegatronBERT
- [Hungarian ModernBERT-base](https://huggingface.co/GaborMadarasz/ModernBERT-base-hungarian) ModernBERT-base pretrained from scratch on ~1B tokens of filtered Hungarian text, 8K context
- [Hun ModernBERT Large](https://huggingface.co/magyar-nlp-szine-java/hun-modernBERT-large-1k) 390M-parameter ModernBERT-large MLM pretrained on Hungarian text
- [huT5](https://huggingface.co/GaborMadarasz/hut5-base) Hungarian-English T5 with a 30K vocabulary (244M parameters, 42% of mT5-base)

### Speech models

- [w2v-BERT 2.0 Hungarian](https://huggingface.co/GaborMadarasz/w2v-bert-2.0-hungarian-CV24.0) Hungarian ASR fine-tune of w2v-BERT 2.0 on Common Voice 24
- [wav2vec2 MMS-1B Hungarian](https://huggingface.co/GaborMadarasz/wav2vec2-large-mms-1b-hungarian) CC0 Hungarian ASR on top of MMS-1B
- [Whisper large-v3 Hungarian LoRA](https://huggingface.co/Maxdorger29/whisper-large-v3-hungarian-lora) LoRA fine-tune packaged for faster-whisper/CTranslate2, reducing Hungarian character and name errors
- [F5-TTS Hungarian](https://huggingface.co/Maxdorger29/f5-tts-hungarian) Hungarian F5-TTS with zero-shot voice cloning from 5-15 seconds of reference audio
- [Diana Hungarian TTS](https://huggingface.co/legekka/diana-hungarian-tts-vits) Single-speaker VITS TTS trained on the KTH Hungarian speech dataset
- [MMS TTS Hungarian](https://huggingface.co/facebook/mms-tts-hun) Hungarian checkpoint of Meta's Massively Multilingual Speech TTS
- [Gemma-3-270M Hungarian ITN](https://huggingface.co/GaborMadarasz/gemma_3_270m_ITN_finetune_16bit) Inverse text normalization of numbers, dates and units in Hungarian ASR output

### Large language models

#### General multilingual large language models

- [Google Gemma 3](https://huggingface.co/blog/gemma3) is a multilingual LLM that also speaks Hungarian
- [EuroLLM](https://huggingface.co/utter-project/models) is a multilingual LLM that also speaks Hungarian
- [gpt-oss](https://gpt-oss.com/) is a multilingual LLM that also speaks Hungarian([Hugging Face](https://huggingface.co/openai/gpt-oss-120b), [GitHub](https://github.com/openai/gpt-oss))

#### Large language models developed for Hungarian use cases

- [PULI-GPTrio](https://huggingface.co/NYTK/PULI-GPTrio) is a Hungarian-English-Chinese trilingual GPT-NeoX model
- [PULI-GPT-3SX](https://huggingface.co/NYTK/PULI-GPT-3SX) is a Hungarian GPT-NeoX model (6.7 billion parameter)
- [PULI-LlumiX-Llama-3.1](https://huggingface.co/NYTK/PULI-LlumiX-Llama-3.1) is an 8B Hungarian-English model built by continually pretraining Llama 3.1 8B on 8.7 billion Hungarian words (16K context)
- [PULI-LlumiX-32K](https://huggingface.co/NYTK/PULI-LlumiX-32K) is a 6.7B Hungarian model built on LLaMA-2-7B-32K with a 32K-token context window
- [PULI-Trio-Q](https://huggingface.co/NYTK/PULI-Trio-Q) is a 7B Hungarian-English-Chinese model built by continually pretraining Qwen2.5-7B on Hungarian data (32K context)
- [PULI-HuBA-130M](https://huggingface.co/NYTK/PULI-HuBA-mamba-130M) is a 130M monolingual Hungarian foundation model based on the Mamba architecture
- [SambaLingo-Hungarian-Base](https://huggingface.co/sambanovasystems/SambaLingo-Hungarian-Base) is a pretrained bilingual Hungarian and English model that adapts Llama-2-7b to Hungarian by training on 59 billion tokens from the Hungarian split of the Cultura-X dataset
- [SambaLingo-Hungarian-Chat](https://huggingface.co/sambanovasystems/SambaLingo-Hungarian-Chat) is a human aligned chat model trained in Hungarian and English
- [PULI-GPT-2](https://huggingface.co/NYTK/PULI-GPT-2) is a Hungarian GPT-2 model
- [OpenEuroLLM-Hungarian](https://ollama.com/jobautomation/OpenEuroLLM-Hungarian) a community Gemma 3 fine-tune published on Ollama under this name, optimized for Hungarian responses (not an official OpenEuroLLM release)
- [Racka 4B](https://huggingface.co/elte-nlp/Racka-4B) is a continually pretrained large language model designed to bridge the resource gap between Hungarian and high-resource languages ([GGUF](https://huggingface.co/elte-nlp/Racka-4B-GGUF))
- [MangaliCa](https://huggingface.co/Obscure-Entropy/MangaliCa) is a Hungarian–English bilingual vision–language model designed for image captioning and image–text retrieval.
- [HunMamba2-780M](https://huggingface.co/magyar-nlp-szine-java/mamba2-780-pretrained) 780M Hungarian Mamba2 language model trained on Europarl and FineWeb-HQ

### LLM Benchmarks

- [HuLU evaluate](https://github.com/nytud/HuLU/tree/master/evaluate) is a library for evaluating and training language models on Hungarian tasks within the HuLU benchmark.
- [OpenHuEval](https://github.com/opendatalab/OpenHuEval) is an LLM benchmark focusing on the Hungarian language.
- [(M)MTEB](https://huggingface.co/spaces/mteb/leaderboard) is a dataset and leaderboard comparing 100+ text embedding models across 1000+ languages including Hungarian.
- [EuroEval](https://euroeval.com/leaderboards/Monolingual/hungarian#__tabbed_1_1) is a language model benchmarking framework that supports evaluating all types of language models out there: encoders, decoders, encoder-decoders, base models, and instruction tuned models.
- [HuGME](https://github.com/nytud/hugme) is an LLM assessment framework that rates the Hungarian language skills and cultural knowledge of models (hallucination, relevance, bias and more).
- [Hu-MMLU](https://huggingface.co/datasets/NYTK/hu-mmlu) is a Hungarian translation and alignment of the MMLU benchmark, organised into one config per subject.
- [HuTruthfulQA](https://huggingface.co/datasets/NYTK/HuTruthfulQA) is a Hungarian truthfulness benchmark with adversarial and non-adversarial questions across 37 categories.
- [HuBoolQ](https://huggingface.co/datasets/NYTK/HuBoolQ) is a Hungarian machine-translated version of BoolQ, keeping the original English, the translation and an optional corrected variant.
- [Hungarian Riddles Benchmark](https://huggingface.co/datasets/boczkakaroly/hungarian-riddles-benchmark) is a riddle-solving benchmark for Hungarian LLMs.
- [Jina Hungarian DocQA](https://huggingface.co/datasets/jinaai/hungarian_doc_qa_beir) is a Hungarian document question answering retrieval benchmark in BEIR format.
- [HuHotpotQA](https://huggingface.co/datasets/GaborMadarasz/HuHotpotQA_8k) 2,259 Hungarian multi-hop question answering examples with supporting facts

## Datasets

### Corpora

- The Hungarian [National Corpus Portal](http://corpus.nytud.hu/nkp/) lists Hungarian corpora with links to their main page _(főoldal)_, concordance _(kereső)_, registration page (if needed, _regisztráció_), and contact e-mail _(kapcsolat)._

#### Raw corpora

- [Hungarian Webcorpus](http://mokk.bme.hu/resources/webcorpus/) An early large Hungarian web corpus, available in its entirety under a permissive Open Content license.
- [Hungarian Webcorpus 2.0](https://hlt.bme.hu/en/resources/webcorpus2) The new version of the Hungarian Webcorpus was built from Common Crawl and includes a little over 9 billion words.
- [OSCAR](https://oscar-project.org/) is a huge multilingual corpus obtained by language classification and filtering of the Common Crawl corpus using the goclassy architecture.
- [emLam](https://hlt.bme.hu/en/resources/emLam) A Language Modeling Benchmark Corpus for Hungarian, similar to the One Billion Word corpus (Chelba, 2014) for English.
- [Leipzig corpora](https://wortschatz.uni-leipzig.de/en/download/) contains randomly selected sentences in the language of the corpus and are available in sizes from 10,000 sentences up to 1 million sentences. The sources are either newspaper texts or texts randomly collected from the web.
- [web2corpus](https://ufal.mff.cuni.cz/w2c) Automatically created multilingual web corpus
- [CC-100](https://data.statmt.org/cc-100) Monolingual Datasets from Web Crawl Data
- [Hungarian fanfiction corpus](https://huggingface.co/datasets/magyar-nlp-szine-java/fanfic) 135M tokens of Hungarian fanfiction split into semantic chunks
- [Hungarian Reddit corpus](https://huggingface.co/datasets/magyar-nlp-szine-java/reddit) 1.07M Hungarian Reddit conversation chunks, 42M tokens
- [Hungarian YouTube comments](https://huggingface.co/datasets/magyar-nlp-szine-java/youtube) 630K Hungarian YouTube comment chunks, 21M tokens
- [hogyankell](https://huggingface.co/datasets/magyar-nlp-szine-java/hogyankell) 2.7K Hungarian how-to articles from hogyankell.hu
- [Hungarian Wikipedia 2025-05-11](https://huggingface.co/datasets/GaborMadarasz/huwiki-20250511) 800K Hungarian Wikipedia articles, 238M tokens, as parquet
- [toxic_oscar_hu](https://huggingface.co/datasets/GaborMadarasz/toxic_oscar_hu) 453M tokens of toxic Hungarian OSCAR text for toxicity training and evaluation

#### Annotated corpora

- [CoNLL 2017: Automatically Annotated Raw Texts and Word Embeddings](https://lindat.mff.cuni.cz/repository/xmlui/handle/11234/1-1989) Automatic segmentation, tokenization and morphological and syntactic annotations of raw texts in 45 languages, generated by [UDPipe](https://ufal.mff.cuni.cz/udpipe), together with word embeddings of dimension 100 computed from lowercased texts by [word2vec](https://code.google.com/archive/p/word2vec/)
- [OpinHuBank](https://sites.google.com/site/mmihaltz/resources) OpinHuBank is a human-annotated corpus to aid the research of opinion mining and sentiment analysis in Hungarian
- [HunEmPoli](https://github.com/uveges/HunEmPoli_corpus) corpus was built using pre-agenda speeches of the Hungarian National Assembly (2014-2018) and consists of 764008 tokens/36475 sentences. Aspect level emotion annotation, with 39840 identified emotions, in addition, marked the keywords that evoked the emotion.
- [The Hungarian forum corpus for Opinion Mining](https://rgai.inf.u-szeged.hu/index.php?lang=en&page=corpus_forum) This database is the first one dedicated to Opinion Mining in Hungarian. The data for further processing were gathered from the posts of the forum topic of the Hungarian government portal dealing with the referendum about dual citizenship.
- [Hungarian sentiment corpus (HuSent)](https://rgai.inf.u-szeged.hu/node/363) is a deeply annotated Hungarian sentiment corpus. It is composed of Hungarian opinion texts written about different types of products, published on the homepage <https://divany.hu/>
- [Szeged Treebank](https://rgai.inf.u-szeged.hu/index.php?lang=en&page=SzegedTreebank) The Szeged Treebank is the largest fully manually annotated treebank of the Hungarian language
- [Szeged Dependency Treebank](https://rgai.inf.u-szeged.hu/index.php?lang=en&page=dependency) The Szeged Dependency Treebank is a dependency-tree format version of the Szeged Treebank.
- [Universal Dependencies](https://github.com/UniversalDependencies/UD_Hungarian)
- [Hungarian Named Entity Corpus](https://rgai.inf.u-szeged.hu/node/130) The Named Entity Corpus for Hungarian is a subcorpus of the Szeged Treebank, which contains full syntactic annotations done manually by linguist experts.
- [KorKor Pilotcorpus](https://github.com/vadno/korkor_pilot) is a gold standard corpus consisting of multiple layers such as dependency parse and coreference annotations
- [NerKor](https://github.com/dlt-rilmta/NerKor) is a gold standard named entity annotated corpus containing 1 million tokens.
- [NerKor 1.41e](https://github.com/novakat/NYTK-NerKor-Cars-OntoNotesPP) A 1M+-token Hungarian named entity dataset with ~30 entity types derived from NYTK-NerKor
- [hunNERwiki](http://hlt.sztaki.hu/resources/hunnerwiki.html) a silver standard corpus for Hungarian Named Entity Recognition
- [Mazsola database](http://corpus.nytud.hu/isz/) contains 28M sentences from the MNSZ1 corpus annotated with shallow syntactic analysis
- [PrevCons](https://github.com/kagnes/prevcons) is a database of 21K hapaxes of verbs with verbal prefixes
- [Hungarian word sense disambiguated corpus](https://rgai.inf.u-szeged.hu/index.php?lang=en&page=corpus_hunwsd) containing 39 suitable word form samples for the purpose of word sense disambiguation
- [HunLearner](https://rgai.inf.u-szeged.hu/index.php?lang=en&page=hunlearner) is a learners' corpus of Hungarian containing written data from 35 students majoring in Hungarian studies at the University of Zagreb, Croatia. Texts were morphologically and syntactically analyzed by the magyarlanc tool.
- [HuLU](https://github.com/nytud/HuLU) Hungarian Language Understanding Benchmark Kit
   - [HuCOLA](https://github.com/nytud/HuCOLA) Hungarian Corpus of Linguistic Acceptability
   - [HuCoPA](https://github.com/nytud/HuCoPA) Hungarian Choice of Plausible Alternatives Corpus
   - [HuCommitmentBank](https://github.com/nytud/HuCommitmentBank) is a corpus of naturally occurring discourses whose final sentence contains a clause-embedding predicate under an entailment canceling operator.
   - [HuSST](https://github.com/nytud/HuSST) Hungarian version of the Sentiment Treebank
   - [HuWNLI](https://github.com/nytud/HuWNLI) Anaphora resolution datasets for Hungarian as an inference task
   - [HuWS](https://github.com/nytud/HuWS) is the Hungarian set of the Winograd schemas
   - [HuRTE](https://github.com/nytud/HuRTE) is the Hungarian version of the Recognizing Textual Entailment datasets
- [HuRC](https://huggingface.co/datasets/NYTK/HuRC) Hungarian Corpus for Reading Comprehension with Commonsense Reasoning
- [ELTE Poetry Corpus](https://github.com/ELTE-DH/poetry-corpus) is a database of complete poems of 50 Hungarian canonical poets together with the sound devices of the poems and the grammatical features of words in XML format
- [ELTE Novel Corpus](https://github.com/ELTE-DH/regenykorpusz) is a database of 400 Hungarian novels (with the annotation of structural units and the grammatical features of words in TEI XML format)
- [ELTE Drama Corpus](https://github.com/ELTE-DH/drama-corpus) is a database of 58 dramas (with the annotation of structural units and the grammatical features of words in TEI XML format)
- [HunSum-1](https://huggingface.co/datasets/SZTAKI-HLT/HunSum-1) is a dataset containing over 1.1M unique news articles with lead and other metadata
- [HAPP](https://github.com/nytud/HAPP) is the Hungarian translation of the Definite Pronoun Resolution Dataset
- [HunSum-2-abstractive](https://huggingface.co/datasets/SZTAKI-HLT/HunSum-2-abstractive) and [HunSum-2-extractive](https://huggingface.co/datasets/SZTAKI-HLT/HunSum-2-extractive) are Hungarian news summarization datasets built from 1.8M articles from 27 news sites
- [HunSimpleNews](https://huggingface.co/datasets/ELTE-DH/HunSimpleNews) is a Hungarian text simplification corpus, containing the standard and simplified versions of whole documents
- [HuAMR](https://huggingface.co/datasets/SZTAKI-HLT/HuAMR) is a Hungarian Abstract Meaning Representation corpus, with 43,810 sentence-AMR pairs ([Llama-3.2-1B-HuAMR](https://huggingface.co/SZTAKI-HLT/Llama-3.2-1B-HuAMR), [mT5-large-HuAMR](https://huggingface.co/SZTAKI-HLT/mT5-large-HuAMR))
- [Hungarian Dialogues](https://huggingface.co/datasets/gedeonmate/Hungarian-Dialogues-text) is a Hungarian dialogue corpus in text form
- [HU_Res_of_Parl_2025_CAP](https://huggingface.co/datasets/poltextlab/HU_Res_of_Parl_2025_CAP) provides CAP annotations for Hungarian parliamentary speeches from 2025
- [Hungarian Folk Song Corpus](https://github.com/ELTE-DH/folk-song-corpus) is a corpus of Hungarian folk songs in TEI XML
- [K-Monitor press database](https://huggingface.co/datasets/K-Monitor/kmdb_base) 66K Hungarian news articles with curated person, institution and place annotations (CC-BY-SA-4.0)
- [kmdb news classification](https://huggingface.co/datasets/K-Monitor/kmdb_classification) 142K Hungarian news articles labelled for corruption and public-spending relevance
- [Hungarian Toxic Comments](https://huggingface.co/datasets/RabidUmarell/hungarian-toxic-comments) 654 manually annotated Hungarian comments scored on five toxicity dimensions
- [Hungarian Reddit conversation threads](https://huggingface.co/datasets/RabidUmarell/hu_reddit_conversation_threads) 72K Hungarian Reddit threads with toxicity labels
- [huReddit toxicity](https://huggingface.co/datasets/RabidUmarell/hureddit-toxicity) Large Hungarian Reddit dataset labelled for toxicity
- [Hungarian coreference corpus](https://huggingface.co/datasets/RabidUmarell/coref-combined) Hungarian coreference chains combined from existing corpora
- [vicc-korpusz](https://huggingface.co/datasets/RabidUmarell/vicc-korpusz) 23K Hungarian jokes with category and rating

#### Parallel corpora

- [Hunglish Corpus](http://mokk.bme.hu/resources/hunglishcorpus/) The Hunglish Corpus is a free sentence-aligned Hungarian-English parallel corpus of about 120 million words in 4 million sentence pairs.
- [SzegedParallel](https://rgai.inf.u-szeged.hu/index.php?lang=en&page=corpus_paralell) The English-Hungarian parallel corpus contains texts selected on the basis of grammatical and translational criteria.
- [HunOr](https://rgai.inf.u-szeged.hu/index.php?lang=en&page=corpus_hunor) A Hungarian-Russian Parallel corpus comprises approximately 800 thousand words.
- [CoNLL 2017 Shared Task Hungarian data](https://lindat.mff.cuni.cz/repository/xmlui/handle/11234/1-1989) Automatic segmentation, tokenization and morphological and syntactic annotations of raw texts from the Common Crawl
- [Hungarian-Russian Prisoner of War Database](https://github.com/dlt-rilmta/hadifogoly-adatbazis)
- [TED talks transcripts parallel corpus](https://www.kaggle.com/db189ab19e7dfeda/ted-talks-transcripts-parallel-corpus) sentence aligned TED talks including Hungarian.
- [TaPaCo Corpus](https://zenodo.org/record/3707949) is a paraphrase corpus for 73 languages, including Hungarian, extracted from the Tatoeba database
- [Duolingo STAPLE](https://sharedtask.duolingo.com/) is a dataset of comprehensive accepted translations from English to 5 different languages, including Hungarian
- [PPDB](https://web.archive.org/web/20231227021302/http://paraphrase.org/#/download) is an automatically extracted database containing millions of paraphrases in 16 different languages, including Hungarian
- [OpenSubtitles Corpus](https://opus.nlpl.eu/legacy/OpenSubtitles/) contains movie subtitles and alignments for 62 languages, including Hungarian
- [OPUS Corpus](https://opus.nlpl.eu) is a growing collection of translated texts from the web
- [MASSIVE dataset](https://github.com/alexa/massive) is a parallel dataset of > 1M utterances across 51 languages with annotations for the Natural Language Understanding tasks of intent prediction and slot annotation.
- [PWS](https://github.com/nytud/PWS) is a parallel collection of the Winograd schemas in seven languages (including Hungarian)
- [parallelbible](https://github.com/nytud/parallelbible) The Parallel Bible Corpus is based on the historical text material of the Old Hungarian Corpus, as its database contains all of the Old and Middle Hungarian Bible translations which are available in this corpus. The King James Bible and three Finnish translations are included in the database as well.

### Linguistic resources

- [morphdb.hu](http://mokk.bme.hu/resources/morphdb-hu/) is an open source morphological database of Hungarian, consisting of a lexicon and morphological grammar that are based on well-founded theoretical decisions.
- [huwn](https://github.com/mmihaltz/huwn) Hungarian Wordnet
- [Hungarian Sentiment Lexicon](https://opendata.hu/dataset/hungarian-sentiment-lexicon) The dictionaries were manually created on the basis of Wordnet-Affect lexicons.
- [poltextLAB's sentiment lexicons](https://web.archive.org/web/20250428042259/https://github.com/poltextlab/sentiment_hun) Highly accurate sentiment lexicons for analysing news data
- [4lang](https://github.com/kornai/4lang) Concept dictionary using Eilenberg machines
- [Named Entity lists for Hungarian](https://rgai.inf.u-szeged.hu/file/69#overlay-context=file/68)
- [Mazsola ISZ](http://corpus.nytud.hu/isz/) lists 500K verb frames extracted from the Mazsola database
- [Manocska](https://github.com/ppke-nlpg/manocska) merges verb frames existing databases
- [PrevLex](https://github.com/kagnes/prevlex) List of phrasal verbs
- [panmorph](https://github.com/dlt-rilmta/panmorph) Tagsets and description of Hungarian morphological analysers.
- [hun_ner_checklist](https://github.com/szegedai/hun_ner_checklist) CHECKLIST diagnostic test cases for Hungarian Named Entity Recognition
- [Hungarian word frequencies](https://huggingface.co/datasets/petyaracz/hungarian-word-frequencies) frequency lists derived from Hungarian web corpora
- [questions-words-hu](http://corpus.nytud.hu/efnilex-vect/data/questions-words-hu.txt) Hungarian analogical questions following Mikolov et al.
- [Hungarian Rhyming Dictionary](https://github.com/ELTE-DH/rhyming-dictionary) is an automatically generated rhyming dictionary of Hungarian canonical poetry

### Linked Open Data

- [Wikipedia dumps](https://dumps.wikimedia.org/huwiki/)
- [Wikidata dumps](https://www.wikidata.org/wiki/Wikidata:Database_download)
- [DBPedia dumps](https://www.dbpedia.org/resources/)
- [huwn.rdf](https://github.com/mmihaltz/huwn.rdf) Hungarian WordNet in RDF format for the Linked Open Data cloud
- [Conceptnet](https://conceptnet.io/) An open, multilingual knowledge graph (with partial Hungarian support)

### Geo data

- [OpenStreetMap (OSM)](https://www.openstreetmap.org/)
  In [Hungary](https://download.geofabrik.de/europe/hungary.html) the [`name`](https://wiki.openstreetmap.org/wiki/Key:name) keys, [otherwise](https://planet.openstreetmap.org/) the [\*name:hu](https://taginfo.openstreetmap.org/search?q=name%3Ahu)
- [Natural-earth-vector](https://github.com/nvkelso/natural-earth-vector) ([`name_hu`](https://github.com/nvkelso/natural-earth-vector/blob/master/packages/Natural_Earth_quick_start/LOCALIZATION.md) imported from wikidata labels)
- [Who's On First](https://whosonfirst.org/) is a gazetteer of places (with [Hungarian administrative places](https://github.com/whosonfirst-data/whosonfirst-data-admin-hu) )

### Speech related data

- [Hungarian Single Speaker Speech Dataset](https://www.kaggle.com/bryanpark/hungarian-single-speaker-speech-dataset)
- [Mozilla Common Voice](https://commonvoice.mozilla.org/hu/datasets)
- [VoxPopuli](https://huggingface.co/datasets/facebook/voxpopuli) 63 hours of transcribed Hungarian speech from European Parliament proceedings (CC0)
- [FLEURS](https://huggingface.co/datasets/google/fleurs) multilingual read-speech benchmark with a Hungarian subset
- [Hungarian Conversational Speech](https://huggingface.co/datasets/SpeechDataAI/hungarian-conversational-speech) conversational Hungarian speech dataset (non-standard license)
- [Hungarian Speech Dataset](https://huggingface.co/datasets/shunyalabs/hungarian-speech-dataset) Hungarian speech dataset (license not stated)
- [CSS10](https://github.com/Kyubyong/css10) A Collection of Single Speaker Speech Datasets for 10 Languages including Hungarian

### Other

- [alpaca_hu_2k](https://huggingface.co/datasets/NYTK/alpaca_hu_2k) is the Hungarian translation of a subset of the Stanford Alpaca prompts.
- [Hungarian synthetic OCR datasets](https://huggingface.co/datasets/GaborMadarasz/synthetic_OCR_dataset_v2) 200K+ generated Hungarian image-text pairs focused on accented characters, and a 205K-pair [MEK variant](https://huggingface.co/datasets/GaborMadarasz/synthetic_OCR_dataset_MEK) mimicking Magyar Elektronikus Könyvtár book typography
- [gsm8k_hungarian_generated_CoT](https://huggingface.co/datasets/GaborMadarasz/gsm8k_hungarian_generated_CoT) Hungarian GSM8K with generated chain-of-thought solutions

## Academy

### Journals

- [Acta Cybernetica](https://www.inf.u-szeged.hu/kutatas/acta-cybernetica)

### Conferences

- [MSZNY](https://rgai.inf.u-szeged.hu/mszny) Conference on Hungarian Computational Linguistics (since 2003)

### Institutes

- [Natural Language Processing Group of the Pázmány Péter Catholic University Faculty of Information Technology and Bionics](https://itk.ppke.hu/)
- [Department of Language Technology and Applied Linguistics, HUN-REN Hungarian Research Centre for Linguistics](https://nytud.hu/kutatocsoport/nyelvtechnologiai-kutatocsoport)
- [Human Language Technology Research Group of the Budapest University of Technology and Economics](https://hlt.bme.hu/en/)
- [Natural Language Processing Group of the University of Szeged](https://rgai.inf.u-szeged.hu/nlp)
- [BME - Laboratory of Speech Acoustics](https://www.tmit.bme.hu/lsa)

## Learning resources

### Books

- [Szövegbányászat](https://www.typotex.hu/book/45/tikk_domonkos_szovegbanyaszat/00)
- [Szövegbányászat és mesterséges intelligencia R-ben](https://tankonyv.poltextlab.com)
- [Kvantitatív szövegelemzés és szövegbányászat a politikatudományban](https://poltextlab.tk.hu/uploads/files/Kvantitativ_szovegelemzes_keszpdf.pdf)

### Courses

- [NLP Courses by the University Of Szeged](https://www.inf.u-szeged.hu/~rfarkas/hallgatok.html)
- [NLP Courses by the HLT Group of the Budapest University of Technology](https://hlt.bme.hu/hu/courses)
- [NLP and Foundation Models lecture slides (ELTE)](https://github.com/elte-nlp/elte-nlp-course)
- [NLP course materials in Hungarian (University of Debrecen)](https://github.com/Clinical-Bioinformatics-Debrecen/nlp_magyar_2025)

### Tutorials

- [Mini NLP Course by the Center Of Digital Humanities](https://pim.hu/hu/digitalis-bolcseszeti-kozpont/nyelvtechnologia-kurzus)
- [Tutorial on Text Mining for Hungarian](https://github.com/oroszgy/hungarian-text-mining-workshop)
- [ai-notebooks](https://github.com/nytud/ai-notebooks) Educational notebooks on language models from NYTK
- [HAIO – Hungarian AI Olympiad](https://github.com/hungarian-ai-olympiad/HAIO-Hungarian-AI-Olympiad) Tasks, solutions and teaching materials from Hungary's national AI olympiad, including Hungarian NLP tasks

## Communities

- [Kereső világ](https://kereses.blog.hu/) Official blog of Precognox Inc.
- [Hungarian NLP Meetup](https://www.meetup.com/hungarian-nlp/)
- [Deep Learning Reading Seminar Meetup](https://www.meetup.com/budapest-deep-learning-reading-seminar/)
- [HuNLP Slack](https://hunlp.slack.com/) Invite required.

## Other Hungarian related resource collections

- [EENLP](https://github.com/altsoph/EENLP) The broad index of NLP resources for Eastern European languages.
- [European Language Grid](https://live.european-language-grid.eu)
- [Hugging Face Datasets (filtered for Hungarian)](https://huggingface.co/datasets?language=language:hu)
- [Awesome LLM Benchmarks HU](https://github.com/latentsubspace/awesome-llm-benchmarks-hu) Curated index of Hungarian and financial sentiment, NER and benchmark datasets
