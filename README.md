# Project Overview

This project is an implementation of face detection and recognition using Python and OpenCV. 
It includes functionalities to read video frames from a webcam, detect faces in real-time, 
save face data, and recognize individuals based on pre-stored datasets. The system uses Haar 
Cascades for face detection and a custom K-Nearest Neighbors (KNN) algorithm for recognition.

## **Components and Functionalities-**

-Video Capture (videoRead.py)
Captures live video feed from a webcam and displays it in real-time.
Ends the capture when the 'q' key is pressed.

-Face Detection (faceDetection.py)
Detects faces in real-time from the video feed using Haar Cascade classifiers.
Draws a rectangle around detected faces and displays the cropped face area.

-Face Data Collection (faceData.py)
Captures face data from the video feed.
Stores face images as numpy arrays in a dataset directory.
Allows user input to assign a name to the captured dataset for recognition purposes.

-Face Recognition (faceRecognition.py)
Loads pre-stored face datasets.
Recognizes faces in real-time using the KNN algorithm.
Displays the name of the recognized person over their face.


## **How It Works-**

Detection:
Haar Cascades detect faces based on trained XML models. Faces are highlighted with bounding boxes in real-time.

Data Collection:
Users can save their face data by providing their name. This is used for training the recognition system.

Recognition:
The collected face data is used to train a KNN model, which matches new inputs to the stored datasets. The recognized name is displayed in the video feed.

## **Steps to run-**

1-First run video read.py to check that your webcam is running or not.

2-Run face_detection.py to check that whether camera is able to capture your face or not, with the help of haar cascase classifier

3-Now, run face_data.py --> this will open up the camera and extract your face from video frames multiple time. Test and store faces of multiple people.

4-At last, run face_recognition.py --> this will detect your face from the dataset made and form a bounding box with you name writtern around your face.
