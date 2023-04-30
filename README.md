# tunisian-signes
Introduction
This project aims to recognize Tunisian Sign Language (TSL) gestures using deep learning and computer vision techniques. The model is trained on a dataset of TSL gestures using LSTM networks, which have shown to be effective in modeling sequential data.

Dataset
The dataset used in this project is a collection of videos of TSL gestures. Each video contains a single gesture performed by a signer. The videos are recorded in various environments with different lighting conditions, camera angles, and backgrounds to increase the model's robustness. The dataset is split into training, validation, and testing sets.

Preprocessing
The videos are preprocessed before feeding them to the LSTM network. First, each frame is extracted from the video and resized to a fixed resolution. Then, the frames are converted to grayscale to reduce the input dimensionality. Finally, the frames are normalized to have zero mean and unit variance.

Model Architecture
The model architecture consists of an LSTM network followed by a fully connected layer with a softmax activation function. The LSTM network is used to model the temporal dependencies between the frames, while the fully connected layer predicts the class of the gesture based on the last hidden state of the LSTM network. The model is trained using the categorical cross-entropy loss function and optimized using the Adam optimizer.

Training
The model is trained on the training set for a fixed number of epochs. The model with the best validation accuracy is saved and used for testing. The training progress is monitored using the training and validation loss and accuracy curves.

Testing
The saved model is tested on the testing set to evaluate its performance. The testing accuracy is reported as the percentage of correctly classified gestures.

Results
The model achieves a testing accuracy of XX% on the TSL dataset. This is a promising result, but there is still room for improvement, especially in handling variations in signer appearance, lighting, and background.

Usage
To use the model for prediction, run the predict.py script with the path to the video file as an argument. The script will preprocess the video frames, feed them to the trained model, and output the predicted gesture class.

Dependencies
Python 3
TensorFlow 2.4
OpenCV
NumPy
Credits
This project was put together as part of my deep learning course. The TSL dataset used in this project was collected and annotated by be influenced by tunisian tiktokers as shown in the videos .
