# 🧠 AI Pneumonia Detector  
*A Deep Learning Tool for Diagnosing Pneumonia from Chest X-rays*

## 📌 Overview
This project was developed as part of the **altREU: Design, Program, and Use Computers to Benefit Society** program.

Pneumonia remains one of the leading causes of death globally, particularly among children. Chest X-rays are a critical tool for detecting pneumonia, but a global shortage of radiology experts often delays accurate diagnosis.

Our solution is an AI-powered pneumonia detector that uses deep learning to analyze chest X-ray images and assist medical professionals by:
- Automatically diagnosing pneumonia
- Highlighting key regions of interest in the lung image using Grad-CAM heatmaps

## 💡 Project Motivation
- Pneumonia is the top cause of infectious death in children worldwide  
- Chest X-rays are widely used but hard to interpret, especially in subtle cases  
- Radiology resources are limited in many regions  
- An AI tool can help bridge this diagnostic gap

## 🧪 Methodology

### 🔍 Dataset
We use the **Chest X-ray Dataset with Lung Segmentation** from [PhysioNet](https://physionet.org/), derived from the **MIMIC-CXR-JPG** dataset. This dataset includes thousands of labeled chest X-rays along with lung segmentation masks to improve model precision.

### 🧠 Model
We implement a **convolutional neural network (CNN)** using the `fastai` library in Python due to its simplicity and effectiveness. Our system:
- Accepts a chest X-ray image as input  
- Outputs a prediction: *Pneumonia* or *Normal*  
- Displays model confidence in the prediction  
- Uses **Grad-CAM** to visualize important regions in the X-ray that influenced the model's decision

### 🛠 Tools & Libraries
- `fastai`  
- `PyTorch`  
- `OpenCV`  
- `NumPy / Pandas`  
- `Matplotlib`  
- `Grad-CAM`

## 📁 Contents
- `pneumonia_detector.ipynb`: Jupyter notebook containing the training, evaluation, and visualization pipeline  
- `Applying Deep Learning Techniques to Classify Pneumonia.pdf`: Research paper detailing model design, performance, and future work

## 🔬 Results
Our model demonstrates promising accuracy and provides intuitive visual explanations through heatmaps, making it suitable for use as a **clinical decision support tool** rather than a replacement for professional radiologists.

## 🎯 Goals
- Provide a reliable second-opinion tool for diagnosing pneumonia from chest X-rays  
- Assist medical professionals, especially in resource-limited settings  
- Explore explainable AI methods in medical imaging

## 🔮 Future Work
- Expand to multi-class classification (e.g., COVID-19, tuberculosis)  
- Improve heatmap resolution and interpretability  
- Deploy as a lightweight web or mobile application
