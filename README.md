# CNN Resnet-50 + LSTM (with Attention) Image Caption Generator Model in Pytorch

## Purpose:
The purpose of this project is to train a deep learning model that consists of a CNN layer being fed as input
to an LSTM layer to predict captions for images. 

## Project Goals:
- Pre-process image dataset to load in Google Colab Jupyter notebook
- Process images to be the same size (256 x 256 RGB), convert to tensors, and normalize them to the Resnet-50 dataset and define all hyperparamets / training arguments.
- Create vocabulary using captions, and pre-process captions to be padded / shortened to 20 tokens long (after tokenization, cleaning to remove one-letter words and punctuation...etc.) and adding start / end tokens.
- Defining the model architecture, importing the Resnet-50 pre-trained model and performing transfer learning.
- Pre-training Word2Vec model and using the embedding tensor as pre-trained weights for the embedding layer
- Connecting the CNN model to the LSTM model using an attention mechanism
- Training and evaluating the model on the given datasets and testing against sample images and calculating bleu scores and accuracy
- Downloading model parameters and integrating an image upload feature for manual user predictions.

## Dataset:
The dataset is obtained from the COCO dataset that can be found and downloaded from the following website. (https://cocodataset.org/#download)

Currently, the dataset used is the 2014 Training / Validation images [83K/13GB] / [41K/6GB] dataset

## How to run project:
More details coming soon once model completes training. The Jupyter notebook found in the repository can be cloned and run from start to finish (so long as the data is downloaded to correct paths) to retrain the model using the same architecture and hyperparameters (this will take ~1 day to complete).

The trained model parameters will be uploaded soon which can be loaded and used directly.
