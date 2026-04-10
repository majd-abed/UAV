# 🚁 UAV Object Detection using YOLO & Faster R-CNN

A deep learning-based object detection system for UAV (drone) imagery, implementing a custom YOLO model from scratch and comparing it with Faster R-CNN.

---

## 📌 Overview

This project focuses on detecting objects in aerial imagery captured by UAVs. It implements:

- 🧠 A custom YOLO (You Only Look Once) model built from scratch in PyTorch  
- 🔍 Faster R-CNN for comparison  
- 📊 Training and evaluation on the **VisDrone dataset**  

The system is optimized for **real-time detection** and designed to handle challenges in aerial imagery such as small objects and dense scenes.

---

## 🚀 Key Features

- 🧠 Custom YOLO architecture (from scratch)  
- 📉 Custom YOLO loss function implementation  
- 🛰️ Trained on UAV dataset (VisDrone)  
- 🔄 Transfer learning from general object detection  
- ⚡ Real-time detection capability  
- ⚖️ Comparison with Faster R-CNN  

---

## 🛠️ Technologies Used

- **Python**
- **PyTorch**
- **Torchvision**
- **OpenCV**
- **NumPy**
- **Matplotlib**

---

## 🧠 Model Architecture

### 🔹 YOLO (Custom Implementation)

- Grid-based detection (S × S)
- Bounding box regression
- Confidence score prediction
- Multi-class classification

Includes:
- Convolutional backbone
- Fully connected detection head
- Custom loss function (localization + confidence + classification)

---

## 📊 Dataset

- **VisDrone Dataset**
  - Designed for UAV-based object detection
  - Contains dense scenes with small objects

---

## 📂 Project Structure


UAV/

│

├── yolo_uav_training.ipynb # YOLO model + training

├── faster_rcnn_uav_experiment.ipynb # Faster R-CNN comparison

│

├── datasets/

├── checkpoints/

└── README.md


---

## ⚙️ Setup

### 1. Clone repository

```bash
git clone https://github.com/majd-abed/UAV.git
cd UAV
2. Install dependencies
pip install torch torchvision matplotlib opencv-python
3. Prepare dataset
Download VisDrone dataset
Place it in your working directory or Google Drive
Update dataset paths in notebooks
▶️ Usage
Train YOLO model

Run:

yolo_uav_training.ipynb
Run Faster R-CNN experiment
faster_rcnn_uav_experiment.ipynb
🧪 Methodology
Load UAV dataset (VisDrone)
Train YOLO model from scratch
Implement custom loss function
Evaluate detection performance
Compare results with Faster R-CNN
📈 Results
YOLO provides faster inference suitable for real-time UAV applications
Faster R-CNN provides higher accuracy but slower performance
⚠️ Challenges
Small object detection
Dense object scenes
Limited UAV-specific data
Computational cost
