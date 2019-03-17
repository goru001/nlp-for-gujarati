# NLP for Gujarati

This repository contains State of the Art Tokenizer, Language model and Classifier for Gujarati, which is a language native to the Indian state of Gujarat.

## Dataset

* Download [Gujarati Wikipedia Articles Dataset](https://drive.google.com/open?id=1yzMEc7BHYq8DCkwYlQHt0-2UzSt1QBZ9) (31,913 articles) which I scraped, cleaned and
used to train the language model

* Download [Gujarati News classification Dataset](https://drive.google.com/open?id=1pwbJuIWyukBoFTvWgn8U2qaCt5JiRVwO) which I scraped and used to train 
the classifier

## Results

#### Language Model

`on 30% validation set`

* Perplexity of language model: ~34

#### Classifier

`On 30% validation set`

* Accuracy of classification model: ~91%
* Kappa score of classification model: ~85

## Pretrained Language Model

Download pretrained Language Model from [here](https://drive.google.com/open?id=1DJ5HskaWs7Fe36nfdXQUWEUyHg_byEz7)


## Classifier

Download classifier from [here](https://drive.google.com/open?id=1cuFxK8P9GIYcSMmTooaoXS3qyjyjuTih)


## Tokenizer

Trained tokenizer using Google's [sentencepiece](https://github.com/google/sentencepiece)

Download the trained model and vocabulary from [here](https://drive.google.com/open?id=1ezarxi-jirgDdy7sShx6VGAuUAJzuT8Q)