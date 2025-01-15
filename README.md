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
The notebook in the repository can be run on google colab to train the network and test it. The weights obtained from training the model are found in the links below and can be loaded in simply by going to the test part of the notebook and loading in the correct checkpoint block. 

The requirements.txt file must be installed prior by running `pip3 install -r requirements.txt` as it contains all dependencies needed for the code to run.

The notebook is written to be used in google colab and make use of the CUDA GPU, but can be run on cpu if needed.

The following pre-trained weights can be uploaded to google colab andd loaded underneath the testing part at the end of the document to use directly without training.

WORD2Vec Model: https://drive.google.com/file/d/1oeHAmjQbiwHnKyJTrjXBWmHwWDJEn92r/view?usp=share_link
Final Model Checkpoint: https://drive.google.com/file/d/1v5eVVmUMBd42DKNBl9HeVUhQt0MjLoGw/view?usp=sharing
