# Tflite Model Maker Workaround 2023
Process for training Tflite Model Maker (EfficientDet) in Google Colab in June/July 2023.

## Background
Google Colab has updated to Python 3.10 which has made the Tflite Model Maker API stop working/load on an infinite loop.

This Colab workbook loads a Conda environment into Google Colab with Python 3.9 and allows for the Tflite Model Maker to be installed and trained.

The working demo is based upon the Android Figurine training example from here:
https://colab.research.google.com/github/khanhlvg/tflite_raspberry_pi/blob/main/object_detection/Train_custom_model_tutorial.ipynb

Edit this process/train.py script as needed for your own training requirements/dataset.

## Detailed Post
The process of how to do this is outlined in this post:

https://discuss.tensorflow.org/t/running-tflite-model-maker-in-google-colab-june-july-2023/18049

## Getting Started

1. [Edit/Build a train.py](train.py) config file to suit your dataset and your training specifications.
2. [Run the colab workbook](Tflite_Model_Maker_Python_3_9.ipynb) to install tflite-model-maker and run the training file.

## On Going

Tensorflow team has pointed out that they are making updates to tflite-model-maker to work with Python 3.10 before they shift over to using Mediapipe as the go to training environment for tflite models.
