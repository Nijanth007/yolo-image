# **Computer Vision Search Engine using YOLO11 + Streamlit**

This repository contains a **Computer Vision Search Engine** built using **YOLO11** for object detection and **Streamlit** for the user interface.  
The system allows users to upload an image and search for objects based on **COCO dataset categories**, visualize predictions, and get bounding-box results in real time.

---

## 🚀 **Features**

- YOLO11-based object detection  
- Supports COCO 80-class object search  
- Streamlit-powered web UI  
- Image upload + object search functionality  
- GPU and CPU setup instructions  
- Modular codebase:
  - `app.py` → Streamlit UI  
  - `inference.py` → Model loading & detection pipeline  
  - `utils.py` → Helper functions  
  - `config.py` → Configurations (paths, thresholds)


## 📦 **Installation Guide**

### **1. Create Environment (GPU)**

```bash
conda create -n yolo_image_search_gpu python=3.11 -y
conda activate yolo_image_search_gpu
conda install pytorch==2.5.1 torchvision==0.20.1 pytorch-cuda=12.4 -c pytorch -c nvidia
pip install -r requirements.txt

