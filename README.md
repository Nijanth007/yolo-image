## YOLO-Based Object Detection System using COCO Dataset

## Introduction

This project implements a real-time object detection system using the YOLO (You Only Look Once) deep learning model trained on the COCO dataset.
The application detects multiple objects in images or video streams with high accuracy and fast inference.
The model is deployed using Streamlit for a simple web-based interface, and experiments are run in VS Code using Conda.

## Dataset & YOLO Model Details (COCO)
Dataset: COCO (Common Objects in Context)

Contains 118,000+ training images

80 object classes (person, car, dog, bus, bottle, etc.)

Used for training many state-of-the-art object detection model
##YOLO Model Used

Model Type: YOLOv5 / YOLOv8 (choose your version)

Pretrained on COCO

Supports:

Real-time inference

Bounding boxes

Class labels

Confidence scores

## Environment Setup
Install Conda (if not installed)

Download from: https://docs.conda.io/en/latest/miniconda.html 
## Create Environment
```
conda create -n yolo_env python=3.10 -y
conda activate yolo_env
```
## Install Required Packages
```
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
pip install ultralytics
pip install streamlit
pip install opencv-python

```
## GPU Installation Steps or CPU Installation Steps

GPU (NVIDIA CUDA) Setup

Install NVIDIA GPU Driver

Install CUDA Toolkit (11.8 recommended)

Install cuDNN

Verify installation

```
nvidia-smi

```
## Install PyTorch with CUDA support

```
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
```
## CPU-Only Setup

```
pip install torch torchvision torchaudio

```
## How to Run in VS Code using Conda
1. Open VS Code
2. Select Conda Environment

Ctrl + Shift + P → Python: Select Interpreter → Choose "yolo_env"

3. Run Script
```
python detect.py --source images/test1.jpg

```
## If using YOLOv8
```
yolo detect predict model=yolov8s.pt source=images/
```
## How to Deploy using Streamlit
Run Streamlit App
```
streamlit run app.py
```
## Output Screenshots
<img width="1916" height="951" alt="image" src="https://github.com/user-attachments/assets/7d02a80b-d8ed-4948-a28c-540c99f050af" />

## Results
Results

Achieved real-time object detection at 30–60 FPS (GPU)

High accuracy due to COCO pretrained YOLO model

Successfully deployed application with Streamlit

User-friendly interface for image/video detection


