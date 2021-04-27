# Anti-Spoof-Face-Recognition
This project addresses a computer vision problem involving face recognition and anti-spoofing methods.

## Objective:
#### The goal is to build face recognition system with an anti-spoof feature. The anti-spoof feature in this project is eye-blink detection. The condition for success is the detection of 5 blinks after a face is recognized. 


## Dataset:
#### The dataset is created by collecting 10-15 pictures of one self and storing it in a folder under the name of the person whose picture it contains.


## Packages:
* OpenCV
* pickle
* imutils
* dlib
* face_recognition
* time
* numpy
* scipy

## Training:
* The training is based on deep metric learning. This involves comparing the the embeddings of a face in the stream to the embeddings of all the faces saved during training. The closest estimated face is given as the output. 
* The training uses the famous ResNet-34 network from the 'Deep Residual Learning of Image Recognition' paper. Albeit, a pre-trained ResNet network with 29 layers and half the filters as the original one was used in the project.
* Basically, the pre-trained model is part of the face_recognition module and can be accessed from there. 
* The face was detected using a CNN that was part of the face_locations function.
* The eye-blink detection involves detecting the face and extracting the eyes and calculating the eye-aspect-ratio.

## Method:


