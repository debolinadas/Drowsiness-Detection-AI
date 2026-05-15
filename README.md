# Drowsiness-Detection-AI
AI-powered Drowsiness Detection system built with Python, TensorFlow, and OpenCV. Real-time driver monitoring with audible sleep alerts.
# Real-Time Drowsiness Detection System
### Deep Learning & Computer Vision Portfolio Project

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/Framework-TensorFlow-orange)](https://www.tensorflow.org/)
[![OpenCV](https://img.shields.io/badge/Library-OpenCV-green)](https://opencv.org/)

## 📌 Project Overview
Driver fatigue is a significant cause of road accidents worldwide. This project implements a real-time computer vision system designed to monitor a driver's eye state and trigger an immediate audible alert if signs of drowsiness (prolonged eye closure) are detected.

By combining **Convolutional Neural Networks (CNN)** with **Haar Cascade Classifiers**, the system achieves a balance between high-speed processing and predictive accuracy.

## 📊 The Data Pipeline
As a data analyst, I structured this project into four distinct phases:
1. **Data Pre-processing**: Images are converted to grayscale and resized to $224 \times 224$ to match the input requirements of the neural network.
2. **Feature Extraction**: Using Haar Cascade files (`haarcascade_frontalface.default.xml` and `haarcascade_eye.xml`) to isolate the Region of Interest (ROI).
3. **Classification**: A trained TensorFlow model classifies the ROI as "Open" or "Closed."
4. **Actionable Logic**: A frame-counter algorithm determines the threshold for "drowsiness" to avoid false positives from natural blinking.

## 🛠️ Technical Stack
* **Language:** Python
* **Deep Learning:** TensorFlow / Keras
* **Computer Vision:** OpenCV
* **Data Manipulation:** NumPy
* **Visualization:** Matplotlib

## 🚀 Key Features
* **Live Video Processing:** Real-time analysis of webcam feeds.
* **Dynamic Alert System:** Uses the `winsound` library to trigger an audio frequency alarm.
* **Visual Feedback:** On-screen status updates ("Open Eyes" vs. "Sleep Alert !!!") with bounding boxes.



## 📁 Repository Structure
```text
├── Major_project_Drow_detect_final.ipynb  # Main Analysis & Execution Notebook
├── requirements.txt                       # Environment Dependencies
├── README.md                              # Project Documentation
└── assets/                                # Haar Cascades and Model files
