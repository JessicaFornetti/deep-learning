# deep-learning

This project is divided into 2 main tasks:

- Task 1: Song Genre Prediction
- Task 2: Image Classification Using Transfer Learning

# Project Overview
This repository contains 3 notebooks, one for [task 1](Deep%20Leaning%20-%20Task%201%20-%20Song%20Genre%20Prediction.ipynb), [task 2](Deep%20Learning%20-%20Task%202%20-%20Image%20Classification%20Using%20Transfer%20Learning.ipynb) and a [demo notebook](Demo%20Notebook.ipynb) to test out the saved models on the test set. 

A [pdf report](Deep%20Learning%20Report.pdf) presents a comparaison of the different results and their analysis.

# Task 1: Song Genre Prediction
This project uses Tensorflow to develop and compare models to predict song genre based on the lyrics only and then based on the lyrics and artist for textual data. To do so the [Multi-Lingual Lyrics for Genre Classification](https://www.kaggle.com/datasets/mateibejan/multilingual-lyrics-for-genre-classification) dataset from Kaggle is used.

A number of models are developped and compared:

- RNN variants (Basic RNN, Single layer LSTM, Multilayer LSTM)
- use of on-the-fly embeddings versus pre-trained embeddings
- traditional text encoding approach (TF-IDF) followed by Logistic Regression
- CNN variants (CNN with same kernel size, different kernel size, CNN as an additional layer before LSTM)
- a non-neural network model (Decision Tree) with hyper parameter tuning

# Task 2: Image Classification Using Transfer Learning

This project uses Tensorflow to predict the image class using the [CIFAR-100 image dataset](https://www.cs.toronto.edu/%7Ekriz/cifar.html). The dataset was randomly split into 2 blocks. Block 1 was used to build various CNN models with the same architecture but varying activation functions, loss functions and the use or not of skip connection as well as an auto encoder model. Transfer learning was applied for block 2 images for the best CNN and auto encoder models, whose weights were saved and then loaded into the demo notebook.

