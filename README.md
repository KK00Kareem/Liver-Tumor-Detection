# Liver-Tumor-Detection
Liver Tumor Detection from MRI Scans (.nii) Using U-Net and SVM This project presents an end-to-end pipeline for automated liver tumor detection using MRI scans in NIfTI (.nii) format. It leverages both machine learning (SVM) and deep learning (U-Net) techniques, supported by detailed voxel-level preprocessing and analysis.

# 🧠 Liver Tumor Detection from MRI Scans (.nii) Using U-Net and SVM

**Bringing AI into medical imaging—one voxel at a time.**

This project presents a complete pipeline for **automated liver tumor detection** from 3D **MRI scans** in **.nii (NIfTI)** format. It combines advanced **voxel-level preprocessing**, **machine learning**, and **deep learning** to classify and segment liver tumors with precision.

---

## 🚀 What It Does

- **Preprocesses volumetric MRI data** to enhance image quality and normalize voxel intensity.
- Uses a **Support Vector Machine (SVM)** to predict tumor presence.
- Implements a **U-Net architecture** to perform voxel-wise semantic segmentation of liver tumors.

---

## 🔧 How It Works

1. **Load .nii Files**  
   Handled with `NiBabel` to access 3D image volumes and metadata.

2. **Preprocessing Steps**  
   - Intensity normalization  
   - Noise reduction via Gaussian filtering  
   - Region of interest extraction  
   - Volume resizing and data augmentation  

3. **Modeling**
   - **SVM**: Trained on extracted features for tumor presence classification.
   - **U-Net**: Trained for precise segmentation of tumor regions.

---

## 🛠️ Tech Stack

- `Python`
- `NumPy`, `OpenCV`, `Matplotlib`
- `NiBabel` – Load and manipulate `.nii` files
- `scikit-learn` – Implement SVM
- `TensorFlow` / `Keras` – Build and train U-Net

---

## 📈 Why It Matters

Liver cancer is one of the most aggressive cancers, often detected too late. This project explores how **AI can support radiologists** by providing fast, scalable, and accurate tumor detection and segmentation—paving the way for earlier diagnosis and better outcomes.

---

## 📌 Future Work

- Upgrade to 3D U-Net for improved volumetric segmentation  
- Add clinical-grade evaluation metrics (Dice, IoU, Hausdorff)  
- Validate on larger, real-world datasets  
- Explore model deployment for research or clinical use
