# Real-Time Facial Emotion Detection 🎭

This project is a **real-time facial emotion detection system** built with **Python, OpenCV and a CNN model (Keras/TensorFlow)**.  
It detects a face from a live camera feed and classifies the emotion into one of **7 categories**:

> 😠 Angry • 🤢 Disgust • 😨 Fear • 😀 Happy • 😐 Neutral • 😢 Sad • 😲 Surprise

---

## 🚀 Features

- Real-time face detection using **OpenCV Haar Cascade**
- Emotion prediction using a **pre-trained CNN model**
- Supports:
  - **Laptop webcam**
  - **Mobile camera** via IP webcam apps
- Easy to run locally with minimal setup
- Simple, readable Python code – good for learning Computer Vision & Deep Learning

---

## 🧠 Model

The model architecture is stored in:

- `facialemotionmodel.json`

The trained weights are stored in:

- `facialemotionmodel.h5`

Input shape: **48 × 48 grayscale** images  
Output: **7 emotion classes** (softmax layer)

These files are loaded in `realtimedetection.py` to perform predictions on each detected face.

---

## 🗂 Project Structure

```bash
Real-Time-Emotion-Detection-/
│
├── train/                     # Training images (by emotion class)
├── test/                      # Testing/validation images (by emotion class)
│
├── facialemotionmodel.json    # Saved model architecture
├── facialemotionmodel.h5      # Saved model weights
│
├── realtimedetection.py       # Main script for real-time emotion detection
├── trainmodel.ipynb           # Notebook used for training the CNN model
│
├── requirements.txt           # Python dependencies
└── README.md                  # Project documentation