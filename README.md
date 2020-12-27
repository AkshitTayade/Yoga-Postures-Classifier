# Yoga Postures Classifier
using MediaPipe &amp; Machine Learning

<img src='https://github.com/google/mediapipe/blob/master/docs/images/mediapipe_small.png' alt='' height=60 width=300>

--------------------------------------------------------------------------------

## Live ML anywhere

[MediaPipe](https://google.github.io/mediapipe/) offers cross-platform, customizable
ML solutions for live and streaming media.

![accelerated.png](https://github.com/google/mediapipe/blob/master/docs/images/accelerated_small.png)                                                               | ![cross_platform.png](https://github.com/google/mediapipe/blob/master/docs/images/cross_platform_small.png)
:------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------:
***End-to-End acceleration***: *Built-in fast ML inference and processing accelerated even on common hardware* | ***Build once, deploy anywhere***: *Unified solution works across Android, iOS, desktop/cloud, web and IoT*
![ready_to_use.png](https://github.com/google/mediapipe/blob/master/docs/images/ready_to_use_small.png)                                                             | ![open_source.png](https://github.com/google/mediapipe/blob/master/docs/images/open_source_small.png)
***Ready-to-use solutions***: *Cutting-edge ML solutions demonstrating full power of the framework*            | ***Free and open source***: *Framework and solutions both under Apache 2.0, fully extensible and customizable*

## MediaPipe in Python

MediaPipe offers customizable Python solutions as a prebuilt Python package on
[PyPI](https://pypi.org/project/mediapipe/), which can be installed simply with
`pip install mediapipe`. It also provides tools for users to build their own
solutions. Please see
[MediaPipe in Python](https://google.github.io/mediapipe/getting_started/python)
for more info.

## MediaPipe solution used in this project
Posture Detection 
<br>
[![pose](https://github.com/google/mediapipe/blob/master/docs/images/mobile/pose_tracking_android_gpu_small.gif)](https://google.github.io/mediapipe/solutions/pose)


## Project Pipeline

### 1. Dataset Collection
 You can collect your own data or use the dataset available [here](https://www.amarchenkova.com/2018/12/04/data-set-convolutional-neural-network-yoga-pose/) 

### 2. Dataset Preparation
 Collect all your images into two folders - Train & Test.
 
 Then iterate over all images and convert each image to its equivalent csv input as shown in this [code](https://github.com/AkshitTayade/Yoga-Postures-Classifier/blob/main/1_DataPreparation.ipynb)
 
 ### 3. Model Making
 After trying lot of ML models, SVM gave the highest accuracy (96%) on Test folder. Model was made using Hyper parameter tunning using GridSearch. [code](https://github.com/AkshitTayade/Yoga-Postures-Classifier/blob/main/2_ModelMaking.ipynb)
 
 ### 4. Testing
 
 According to the Test folder, all the images were correctly classified. [code](https://github.com/AkshitTayade/Yoga-Postures-Classifier/blob/main/3_Testing.ipynb)
 
 <p align="center">
  <img width="460" height="300" src="https://github.com/AkshitTayade/Yoga-Postures-Classifier/blob/main/Images/Screenshot%202020-12-27%20at%206.00.18%20PM.png">
  <img width="460" height="300" src="https://github.com/AkshitTayade/Yoga-Postures-Classifier/blob/main/Images/Screenshot%202020-12-27%20at%206.00.23%20PM.png">
</p>
 
<p align="center">
  <img width="460" height="300" src="https://github.com/AkshitTayade/Yoga-Postures-Classifier/blob/main/Images/Screenshot%202020-12-27%20at%206.00.28%20PM.png">
  <img width="460" height="300" src="https://github.com/AkshitTayade/Yoga-Postures-Classifier/blob/main/Images/Screenshot%202020-12-27%20at%206.00.32%20PM.png">
</p>

<p align="center">
  <img width="460" height="300" src="https://github.com/AkshitTayade/Yoga-Postures-Classifier/blob/main/Images/Screenshot%202020-12-27%20at%206.01.26%20PM.png">
  <img width="460" height="300" src="https://github.com/AkshitTayade/Yoga-Postures-Classifier/blob/main/Images/Screenshot%202020-12-27%20at%206.01.35%20PM.png">
</p>
 

 > This project was performed using Google Colab.
 
 ## Advantange of my procedure over Deep learning Models
 * Deep learning models take very long time to train
 * Computional needs are very less
 * My model trains in less than 2 seconds
 * Training accuracy was lower than Testing accuracy, which indicates the model has learned perfectly and haven't overfitted.
 
