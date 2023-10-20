# Tunisian Signes

## Introduction
This project aims to recognize Tunisian Sign Language (TSL) gestures using deep learning and computer vision techniques. The model is trained on a dataset of TSL gestures using LSTM networks, which have shown to be effective in modeling sequential data.

## Dataset
The dataset used in this project is a collection of videos of TSL gestures recorded by the author. Each video contains a single gesture performed by a signer. The videos are recorded in various environments with different lighting conditions, camera angles, and backgrounds to increase the model's robustness. The dataset is split into training, validation, and testing sets.

## Preprocessing
The videos are preprocessed before feeding them to the LSTM network. First, each frame is extracted from the video and resized to a fixed resolution. Then, the frames are converted to grayscale to reduce the input dimensionality. Finally, the frames are normalized to have zero mean and unit variance.

## Tunisian Sign Language Recognition System
This project aims to design and develop a system for real-time recognition and interpretation of Tunisian Sign Language (TSL) using computer vision and deep learning techniques. The system utilizes advanced technologies such as LSTM and the Mediapipe library to achieve accurate gesture classification.

## Model Architecture
The model architecture consists of an LSTM network followed by a fully connected layer with a softmax activation function. The LSTM network is used to model the temporal dependencies between the frames, while the fully connected layer predicts the class of the gesture based on the last hidden state of the LSTM network. The model is trained using the categorical cross-entropy loss function and optimized using the Adam optimizer.

## Features
- **Real-time recognition:** The system is capable of analyzing TSL gestures in real-time, providing immediate feedback and interpretation.
- **Computer vision:** Computer vision techniques are employed to detect and track hand movements and gestures.
- **Deep learning:** The system utilizes a deep learning model, specifically an LSTM (Long Short-Term Memory) network, to classify the detected gestures into corresponding TSL signs.
- **Mediapipe integration:** The project leverages the Mediapipe library, a powerful framework for building multimodal applied machine learning pipelines, to streamline the processing of video inputs and hand tracking.

## Dependencies
- Python 3
- TensorFlow 2.4
- OpenCV
- NumPy

## Credits
This project was put together as part of my deep learning course. The TSL dataset used in this project was collected and annotated by be influenced by Tunisian TikTokers as shown in the videos.

Enjoy real-time Tunisian Sign Language recognition!

## Contributing
Contributions are welcome! If you have any ideas or suggestions for improvement, please submit a pull request. For major changes, please open an issue first to discuss potential updates.
