# 🧠 Age and Gender Detection

A computer vision project that detects human **age** and **gender** from facial images using deep learning and OpenCV.

## 📌 Overview

This project leverages pre-trained deep learning models to detect human faces from an image or webcam feed, and then predict:

- 🧓 Estimated **Age Group**  
- 🚻 Predicted **Gender** (Male/Female)

It uses OpenCV's DNN module and deploys models trained on large datasets for high accuracy.

---

## 🎯 Features

- 📸 Real-time face detection from webcam or image
- 🧬 Predicts age groups like: `0-2`, `4-6`, `8-12`, `15-20`, `25-32`, `38-43`, `48-53`, `60-100`
- 🚹🚺 Gender classification: `Male` or `Female`
- 🔁 Easily extendable to support multiple faces in a single frame

---

## 🛠️ Technologies Used

- 🧠 **OpenCV** (DNN module)
- 🖼️ **Pre-trained Caffe Models**
- 🐍 **Python 3.x**

---

## 🗂️ File Structure
```
Age-and-Gender-Detection/
│
├── age_deploy.prototxt        # Model architecture for age detection
├── age_net.caffemodel         # Pre-trained age model
├── gender_deploy.prototxt     # Model architecture for gender detection
├── gender_net.caffemodel      # Pre-trained gender model
├── sample.jpg                 # Sample image input
├── detect.py                  # Main script for detection
└── README.md                  # Project documentation
```


---

## ▶️ How to Run

### 🔧 Requirements

Install the necessary packages:

```bash
pip install opencv-python
```

📷 Run on Sample Image
```bash
python detect.py --image sample.jpg
```


🎥 Run on Webcam
```bash
python detect.py
```


📊 Age Groups Defined in Model

```
['(0-2)', '(4-6)', '(8-12)', '(15-20)', 
 '(25-32)', '(38-43)', '(48-53)', '(60-100)']
```


📦 Pretrained Models

The models used are from:
	•	Age & Gender Classification using OpenCV DNN with Caffe Models
These are based on convolutional neural networks (CNNs) trained on the IMDB-WIKI and Adience datasets.




