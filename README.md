# NLP for Gujarati

This repository contains State of the Art Language models and Classifier
 for Gujarati, which is a language native to the Indian state of Gujarat.

The models trained here have been used in [Natural Language Toolkit for Indic Languages
 (iNLTK)](https://github.com/goru001/inltk)

## Dataset

#### Created as part of this project
1. [Gujarati Wikipedia Articles](https://www.kaggle.com/disisbig/gujarati-wikipedia-articles)

2. [Gujarati News Dataset](https://www.kaggle.com/disisbig/gujarati-news-dataset)

#### Open Source Datasets
1. [iNLTK Headlines Corpus - Gujarati](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets) : Uses the Gujarati News Dataset prepared above.


## Results

### Language Model Perplexity (on validation set)

| Architecture/Dataset | Gujarati Wikipedia Articles |
|:--------:|:----:|
|   ULMFiT  |  34.12  |
|  TransformerXL |  28.12  |


### Classification Metrics

##### ULMFiT


| Dataset | Accuracy | MCC | Notebook to Reproduce results |
|:--------:|:----:|:----:|:----:|
| iNLTK Headlines Corpus - Gujarati | 91.05  |  86.09  | [Link](https://github.com/goru001/nlp-for-gujarati/blob/master/classification/Gujarati_Classification_Model.ipynb) |
 

### Visualizations
 
##### Word Embeddings

| Architecture | Visualization |
|:--------:|:----:|
| ULMFiT | [Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-gujarati/master/language-model/embedding_projector_config.json) |
| TransformerXL | [Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-gujarati/master/language-model/embedding_projector_transformer_config.json)  |



### Results of using Transfer Learning + Data Augmentation from iNLTK

##### On using complete training set (with Transfer learning)

| Dataset | Dataset size (train, valid, test) | Accuracy | MCC | Notebook to Reproduce results |
|:--------:|:----:|:----:|:----:|:----:|
| iNLTK Headlines Corpus - Gujarati | (5269, 659, 659) | 91.05 | 86.09 | [Link](https://github.com/goru001/nlp-for-gujarati/blob/master/classification/Gujarati_Classification_Model.ipynb) |
 

##### On using 10% of training set (with Transfer learning)

| Dataset | Dataset size (train, valid, test) | Accuracy | MCC | Notebook to Reproduce results |
|:--------:|:----:|:----:|:----:|:----:|
| iNLTK Headlines Corpus - Gujarati | (526, 659, 659) | 80.88 | 70.18 | [Link](https://github.com/goru001/nlp-for-gujarati/blob/master/classification/Gujarati_Classification_Model_without_aug.ipynb) |
 
##### On using 10% of training set (with Transfer learning + Data Augmentation)

| Dataset | Dataset size (train, valid, test) | Accuracy | MCC | Notebook to Reproduce results |
|:--------:|:----:|:----:|:----:|:----:|
| iNLTK Headlines Corpus - Gujarati | (526, 659, 659) | 81.03 | 70.44 | [Link](https://github.com/goru001/nlp-for-gujarati/blob/master/classification/Gujarati_Classification_Model_with_aug.ipynb) |


## Pretrained Models

#### Language Models 

Download pretrained Language Models from [here](https://drive.google.com/open?id=1DJ5HskaWs7Fe36nfdXQUWEUyHg_byEz7)

#### Tokenizer

Trained tokenizer using Google's [sentencepiece](https://github.com/google/sentencepiece)

Download the trained model and vocabulary from [here](https://drive.google.com/open?id=1ezarxi-jirgDdy7sShx6VGAuUAJzuT8Q)
