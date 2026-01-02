


# 💵 Fake Currency Detection System Using CNN and Computer Vision

A GUI-based Fake Currency Detection System that analyzes Indian currency notes using **Computer Vision techniques** with an **extendable CNN-based classification pipeline**.  
The system verifies multiple **security features** of currency notes and presents **feature-wise analysis with PASS/FAIL status** through an interactive interface.

---

## 📌 Project Description

Counterfeit currency is a major challenge to financial security.  
This project implements a **feature-driven fake currency detection system** that examines **visual security elements** of Indian currency notes (₹500 and ₹2000).

The system is divided into:
1. **Starting GUI** – Image selection & currency type
2. **Detection Engine** – Feature extraction and verification
3. **Ending GUI** – Feature-wise result visualization

A **CNN-based model** is proposed as an extensible module for intelligent classification and future enhancement.

---

## 🧠 Core Features

- ✔️ Detection of fake currency notes using image processing
- ✔️ Analysis of **multiple security features**
- ✔️ Feature-wise **PASS / FAIL** evaluation
- ✔️ ORB + SSIM similarity matching
- ✔️ Bleed line detection (left & right)
- ✔️ Serial number character analysis
- ✔️ Scrollable Tkinter GUI
- ✔️ Modular and explainable design

---

## 🛠️ Technologies Used

- **Python**
- **OpenCV**
- **NumPy**
- **Tkinter**
- **Pillow (PIL)**
- **Matplotlib**
- **Scikit-image (SSIM)**
- **CNN (Design-ready / Extensible module)**

---

## 📁 Repository Structure

```

├── .ipynb_checkpoints/
├── Dataset/
│   └── Fake Notes/
├── In/
│   ├── 500 Testing.ipynb
│   ├── 2000 Testing.ipynb
│   ├── controller.ipynb
│   ├── gui 1.ipynb
│   ├── gui 2.ipynb
│   ├── Untitled.ipynb
│   ├── Image_not_found.jpg
│   └── FAKE CURRENCY DETECTOR REPORT.pdf

```

---

## 🧩 System Workflow

```

User Input Image
↓
GUI (Image Selection & Currency Type)
↓
Preprocessing (Resize, Color Conversion)
↓
Feature Extraction & Matching
├── ORB + SSIM (Visual Features)
├── Bleed Line Detection
└── Serial Number Analysis
↓
Rule-Based Decision Logic
↓
Result Visualization (Ending GUI)

````

---

## 🔍 Security Features Analyzed

| Feature Category | Description |
|-----------------|-------------|
| Structural Features | ORB + SSIM-based pattern similarity |
| Bleed Lines | Left and Right edge detection |
| Serial Number | Character count verification |
| Overall Decision | Feature aggregation logic |

---

## 🖥️ Graphical User Interface

### 🔹 Starting GUI
- Allows users to:
  - Select currency image from system
  - Choose denomination (₹500 / ₹2000)
  - Submit image for analysis

### 🔹 Ending GUI
- Displays:
  - Input image
  - Feature-wise extracted images
  - Similarity scores and statistics
  - PASS / FAIL status for each feature
  - Final authenticity result

---

## ▶️ How to Run the Project

### 1️⃣ Install Required Libraries
```bash
pip install opencv-python numpy pillow matplotlib scikit-image
````

### 2️⃣ Run Notebooks

Open Jupyter Notebook and execute in the following order:

1. `gui 1.ipynb` → Starting GUI
2. `controller.ipynb` → Feature extraction & analysis
3. `gui 2.ipynb` → Result visualization

---

## 🧪 CNN Module (Proposed)

* CNN can be integrated to:

  * Classify notes as **Genuine / Fake**
  * Improve robustness over handcrafted features
* Intended for future work and research extension

> This hybrid approach improves **accuracy + explainability**, making it suitable for academic projects.

---

## 🎓 Academic Relevance

* Final Year Engineering Project
* Computer Vision / Image Processing
* AI-based Security Applications
* Suitable for IEEE conference submissions

---

## 🚀 Future Enhancements

* Full CNN training and deployment
* Support for additional denominations
* Real-time camera input
* Web or mobile application
* Dataset expansion and augmentation



