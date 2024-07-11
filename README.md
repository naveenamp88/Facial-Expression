# Real-Time Facial Expression Recognition_Palanichamy Naveen

## Introduction
This project demonstrates a real-time facial expression recognition system using deep learning. The system captures video from a webcam, detects faces, and classifies their expressions into categories such as Angry, Disgust, Fear, Happy, Sad, Surprise, and Neutral.

## Dataset
The project uses a pre-trained model for facial expression recognition. The model is loaded from an HDF5 file (`emotion_model.hdf5`). 
**Link**: https://github.com/dinuduke/Facial-Emotion-Recognition/blob/master/models/emotion_model.hdf5

## Steps

1. **Loading the Model**: We load the pre-trained model and compile it to ensure compatibility with the current version of TensorFlow.
2. **Capturing Video**: We use OpenCV to capture real-time video from the webcam.
3. **Processing Frames**: Each frame is converted to grayscale, and faces are detected using OpenCV's Haar Cascade.
4. **Predicting Emotions**: The detected faces are resized to the input size expected by the model, normalized, and then fed into the model to predict the emotion.
5. **Displaying Results**: The detected faces are highlighted with rectangles, and the predicted emotion labels are displayed on the video feed.
6. **Exiting the Loop**: The video feed can be exited by pressing the 'q' key.

## Installation

To run this project, you need Python installed along with the following libraries:
- `tensorflow`
- `opencv-python`
- `numpy`

You can install these libraries using pip:

```sh
pip install tensorflow opencv-python numpy
