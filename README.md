# HAND-GESTURE-RECOGINITION-SYSTEM-FOR-DEAF-AND-DUMB-COMMUNICATION
A User Friendly dashboard for the hand gestures 
Real-time Hand Gesture Recognition using TensorFlow & OpenCV
Gesture recognition is an active research field in Human-Computer Interaction technology. It has many applications in virtual environment control and sign language translation, robot control, or music creation. In this machine learning project on Hand Gesture Recognition, we are going to make a real-time Hand Gesture Recognizer using the Media Pipe framework and TensorFlow in OpenCV and Python.
OpenCV is a real-time Computer vision and image-processing framework built on C/C++. But we’ll use it on python via the OpenCV-python package.
What is Media Pipe?
Media Pipe is a customizable machine learning solutions framework developed by Google. It is an open-source and cross-platform framework, and it is very lightweight. Media Pipe comes with some pre-trained ML solutions such as face detection, pose estimation, hand recognition, object detection, etc.
What is TensorFlow?
TensorFlow is an open-source library for machine learning and deep learning developed by the Google brains team. It can be used across a range of tasks but has a particular focus on deep neural networks.
Neural Networks are also known as artificial neural networks. It is a subset of machine learning and the heart of deep learning algorithms. The concept of Neural networks is inspired by the human brain. It mimics the way that biological neurons send signals to one another. Neural networks are composed of node layers, containing an input layer, one or more hidden layers, and an output layer.
 
•	Mp.solution.hands module performs the hand recognition algorithm. So we create the object and store it in mpHands.
•	Using mpHands.Hands method we configured the model. The first argument is max_num_hands, that means the maximum number of hand will be detected by the model in a single frame. Media Pipe can detect multiple hands in a single frame, but we’ll detect only one hand at a time in this project.
•	Mp.solutions.drawing_utils will draw the detected key points for us so that we don’t have to draw them manually.

•	Using the load_model function we load the TensorFlow pre-trained model.
•	Gesture.names file contains the name of the gesture classes. So first we open the file using python’s inbuilt open function and then read the file.
•	After that, we read the file using the read() function.
•	We create a Video Capture object and pass an argument ‘0’. It is the camera ID of the system. In this case, we have 1 webcam connected with the system. If you have multiple webcams then change the argument according to your camera ID. Otherwise, leave it default.
•	The cap.read() function reads each frame from the webcam.
•	cv2.flip() function flips the frame.
•	cv2.imshow() shows frame on a new OpenCV window.
•	The cv2.waitKey() function keeps the window open until the key ‘q’ is pressed.


