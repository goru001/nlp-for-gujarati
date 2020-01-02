# NLP for Gujarati

This repository contains State of the Art Language models and Classifier
 for Gujarati, which is a language native to the Indian state of Gujarat.

The models trained here have been used in [Natural Language Toolkit for Indic Languages
 (iNLTK)](https://github.com/goru001/inltk)

## Dataset

#### Created as part of this project
1. [Gujarati Wikipedia Articles](https://www.kaggle.com/disisbig/gujarati-wikipedia-articles)

2. [Gujarati News Dataset](https://www.kaggle.com/disisbig/gujarati-news-dataset)

## Results

#### Language Model Perplexity

| Architecture/Dataset | Gujarati Wikipedia Articles |
|:--------:|:----:|
|   ULMFiT  |  34.12  |
|  TransformerXL |  28.12  |


#### Classification Metrics

##### ULMFiT

| Dataset | Accuracy | Kappa Score |
|:--------:|:----:|:----:|
| Gujarati News Dataset |  92.4  |  87.9  |

#### Visualizations
 
##### Embedding Space

| Architecture | Visualization |
|:--------:|:----:|
| ULMFiT | [Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-gujarati/master/language-model/embedding_projector_config.json) |
| TransformerXL | [Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-gujarati/master/language-model/embedding_projector_transformer_config.json)  |


## Pretrained Language Model

Download pretrained Language Model from [here](https://drive.google.com/open?id=1DJ5HskaWs7Fe36nfdXQUWEUyHg_byEz7)


## Classifier

Download classifier from [here](https://drive.google.com/open?id=1cuFxK8P9GIYcSMmTooaoXS3qyjyjuTih)


## Tokenizer

Trained tokenizer using Google's [sentencepiece](https://github.com/google/sentencepiece)

Download the trained model and vocabulary from [here](https://drive.google.com/open?id=1ezarxi-jirgDdy7sShx6VGAuUAJzuT8Q)