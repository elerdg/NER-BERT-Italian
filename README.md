## Named Entity Recognition with BERT on Italian  

This project aims to fine-tune pre-trained BERT models for named-entity recognition (NER) on Italian Data from the  [Wikineural Dataset](https://github.com/Babelscape/wikineural/tree/master/data/wikineural/it)

## Overview:
- fine-tune the pre-trained BERT models:
  - [bert-base-multilingual-cased](https://huggingface.co/bert-base-multilingual-cased) 
  - [bert-base-italian-cased](https://huggingface.co/dbmdz/bert-base-italian-cased) 

- test the fine-tuned BERT models for NER on:
  - sentences from the **validation set** of the Italian [Wikineural Dataset](https://github.com/Babelscape/wikineural/tree/master/data/wikineural/it)
  - **sentences predicted** by the pre-trained model **wav2vec2-xls-r fine-tuned on Italian data for ASR**

## The dataset:
[Wikineural IT](https://github.com/Babelscape/wikineural/tree/master/data/wikineural/it) comprises 111k sentences from Wikipedia, tokenized and ner tagged. The Dataset is organized in 3 splits: train, test, and validation. The sentences are cased and contain punctuation. The **entity categories** are  encoded as illustrated below:  
```
{'O': 0, 'B-PER': 1, 'I-PER': 2, 'B-ORG': 3, 'I-ORG': 4, 'B-LOC': 5, 'I-LOC': 6, 'B-MISC': 7, 'I-MISC': 8}
```
## The pre-trained models in this project: 
  - [bert-base-multilingual-cased](https://huggingface.co/bert-base-multilingual-cased) pre-trained on 104 languages with the largest Wikipedia Dataset.  
  - [bert-base-italian-cased](https://huggingface.co/dbmdz/bert-base-italian-cased) pre-trained on Wikipedia texts and OPUS corpora for a total Corpus of the size of 13GB.

