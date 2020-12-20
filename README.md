# Face-recogniser-using-Deep-Learning
## Introduction
This project is a image based capturing system using deep learning and computer vision.This system recognize a person image and give the result whether it is a match or no match
It's a deep neural network from scratch.The language used is Python and Keras libraries are utilized for neural network.For face extraction MTCNN is used.
For complete code visit the code page of this repository
## Requirements
This project requires some modules to import which are
1.import numpy as np 
2.import pandas as pd
3.import os
4.import cv2
5.from mtcnn.mtcnn import MTCNN
6.from keras.utils import to_categorical
7.from sklearn.preprocessing import LabelEncoder
8.from keras.models import Model
9.from keras.layers import *
10.from keras.regularizers import *
11.from keras.optimizers import RMSprop
12.import tensorflow as tf
13.from tensorflow import keras
14.from tensorflow.keras import layers
15.from tensorflow.keras.models import Sequential
## Installations
 pip needs to be install which is
pip install mtcnn
## Description
So we have to make the arrangements for croppingout the face from the image which can be done by the library MTCNN. It helps in detecting bounding box of face in a image. We will use that bounding box to crop the image and store it. To use the MTCNN pip of mtcnn needs to be install.Then we use our dataset to store the images in our program.In this program ,dataset is used in which passport size of a person notated with script  is stored and other its two photo of that person matched with it or not is checked by this program.This deep learning model  use a skip function to retain our input image features for deeper layers. We will define a single block of 3 convolutional layers with Batch normalization in between them and apply Add function on input layer for the block and output layer of the current block. With increasing filters in each block. We will add 10 such blocks to with filters starting from 64 to 4096. Though you can change the number of filters to reduce computation but there might be chances of decrease in accuracy.We will use RMSprop as optimizer and Adam can also be used but by experiment better accuracy is given by RMSprop optimizer.We used data augmentation also.Then we have to train our model which shows the accuracy.
## Usage
This project can be used in attendance system for employees in office and students in school.It also be used as a face password.
