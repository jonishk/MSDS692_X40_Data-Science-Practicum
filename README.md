# 🧠 Brain Tumor Multimodal Image Classification (CT + MRI)

This repository contains the code, models, and visualizations for a deep learning-based project to classify brain tumor images using both CT and MRI scans. The project demonstrates the power of **multimodal fusion learning** in the healthcare domain, specifically in early tumor detection.

## 📌 Project Overview

This project aims to:
- Build two separate CNN models for CT and MRI image classification.
- Fuse both modalities to create a more robust **multimodal classification model**.
- Evaluate performance using metrics like Accuracy, Precision, Recall, F1 Score, and Confusion Matrix.

✅ Final Practicum Submission for **MSDS692 – Data Science Practicum**  
🎓 Regis University  
👨‍💻 Author: Jonish Bishwakarma
Google colab: https://colab.research.google.com/drive/157S471g4zYT4ij0uazLak67DYBNX1G7B?usp=sharing

 

---

## 📂 Dataset

Dataset used: [Brain Tumor Multimodal Image (CT & MRI)](https://www.kaggle.com/datasets/murtozalikhon/brain-tumor-multimodal-image-ct-and-mri)

**Structure:**
Dataset/
├── Brain Tumor CT scan Images/
│ ├── Healthy/
│ └── Tumor/
├── Brain Tumor MRI images/
│ ├── Healthy/
│ └── Tumor/


Each folder contains `.jpg`, `.png`, and `.jpeg` formatted medical scan images categorized as either `Healthy` or `Tumor`.

---

## ⚙️ Project Pipeline

1. **Data Preprocessing**
   - Image resizing (224x224), normalization
   - Train/test split (80/20)
2. **Exploratory Data Analysis**
   - Sample image visualizations
   - Class distributions
   - Format statistics
3. **Model Architecture**
   - Custom CNN for CT and MRI
   - Late fusion via concatenation
4. **Training**
   - Epochs: 10
   - Optimizer: Adam
   - Loss: CrossEntropy
5. **Evaluation**
   - Classification Report
   - Confusion Matrix
   - Visual prediction grid

---

## 🧠 Model Architecture

- **CT Model** → CNN  
- **MRI Model** → CNN  
- **Fusion** → Concatenated features passed to dense layers  
- **Output** → Binary classifier (Healthy / Tumor)

> Detailed architecture is available in the notebook:  
> `Jonish_MSDS692_Practicum.ipynb`

---

## 🚀 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/brain-tumor-multimodal-classification.git
   cd brain-tumor-multimodal-classification

## 📄 License
This project is for academic and educational purposes only.
