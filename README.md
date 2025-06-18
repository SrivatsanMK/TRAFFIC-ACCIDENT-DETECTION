# ABSTRACT

Accurate and timely detection of road accidents is crucial for enhancing road safety and minimizing potential hazards. In this project, we present an advanced Accident 
Detection Model based on a state-of-the-art real-time object detection framework. Our model utilizes computer vision techniques to analyze road surveillance videos, identify 
potential accidents, and provide proactive insights for risk mitigation. The predictive component of the system utilizes a machine learning model trained on a diverse dataset of
historical accident data, considering factors like as road geometry. The model learns to recognize patterns and correlations between these factors and the occurrence of 
accidents. As a result, it can predict the probability of an accident happening in real-time based on the ongoing video feed.The user interface provides a straightforward and 
intuitive platform for users to upload road CCTV videos and receive instantaneous feedback regarding the likelihood of an accident. The system gives the output of the video by 
input video as either accident occurs or not with a corresponding confidence score. Users can thus take proactive measures to mitigate potential risks and enhance overall road 
safety.The proposed Intelligent Accident Prediction System aims to contribute to the reduction of road accidents by providing a proactive and data-driven approach to 
identifying potential risk factors. By integrating cutting-edge computer vision technologies, this system represents a step towards the development of smarter, safer, and 
more efficient transportation systems. The project concludes with the deployment of the trained model for accident detection on external videos. Users can input video, and the 
model processes and identifies potential accidents.

# Accident Detection System

1. Demonstration
2. What is Accident Detection System?
3. Prerequisites
4. Getting Started- How to use it?
5. Description
6. Future Work

## 1. Demonstration

![Demo](https://user-images.githubusercontent.com/54409969/173066273-732f7da9-8645-4809-aa7a-bb2f78548b3e.gif)

## 2. What is Accident Detection System?

An accident Detection System is designed to detect accidents via video or CCTV footage. Road accidents are a significant problem for the whole world. Many people lose their lives in road accidents. We can minimize this issue by using CCTV accident detection. This repository majorly explores how CCTV can detect these accidents with the help of Deep Learning.

## 3. Prerequisites

- To use this project Python Version > 3.6 is recommended.
- To contribute to this project, knowledge of basic python scripting, Machine Learning, and Deep Learning will help.

## 4. Getting Started - How to use it?

### Clone this repository
```bash
git clone https://github.com/SrivatsanMK/TRAFFIC-ACCIDENT-DETECTION.git
```

To install all the packages required to run this python program
`pip install -r requirements.txt`

**Note:** This project requires a camera. So make sure you have a connected camera to your device. You can also use a downloaded video if not using a camera.

### Run
Before running the program, you need to run the `accident-classification.ipynb` file which will create the `model_weights.h5` file. Then, to run this python program, you need to execute the `main.py` python file.

## 5. Description

This program includes 4 things.

1. `data`: Kaggle dataset on [Accident Detection from CCTV footage](https://www.kaggle.com/code/mrcruise/accident-classification/data).
2. `accident-classification.ipynb`: This is a jupyter notebook that generates a model to classify the above data. This file generates two important files `model.json` and `model_weights.h5`.
3. `detection.py`: This file loads the Accident Detection system with the help of `model.json` and `model_weights.h5` files.
4. `camera.py`: It packs the camera and executes the `detection.py` file on the video dividing it frame by frame and displaying the percentage of the prediction in the accident (if present) in the frame.

## 6. Future Work

We can use an alarm system that can call the nearest police station in case of an accident and also alert them of the severity of the accident.
