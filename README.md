
# 💵 Fake Currency Detection System Using CNN

A hybrid **Computer Vision + Convolutional Neural Network (CNN)** based system for detecting **fake Indian ₹500 currency notes**.  
The system analyzes multiple **currency security features**, provides **feature-wise pass/fail results**, and delivers an **overall authenticity decision** through an interactive GUI.

---

## 📌 Project Overview

Counterfeit currency is a major economic and security concern.  
This project presents a **multi-stage fake currency detection system** that combines:

- **Classical Computer Vision techniques** for explainable feature verification  
- **CNN-based learning (extensible module)** for intelligent classification  
- **GUI-based interaction** for ease of use

The system validates currency authenticity by examining **10 critical security features** commonly found in genuine Indian ₹500 notes.

---

## 🧠 Key Highlights

- ✔️ Hybrid **CNN + Rule-Based CV Architecture**
- ✔️ Analysis of **10 currency security features**
- ✔️ Feature-wise **PASS / FAIL** classification
- ✔️ ORB + SSIM similarity matching
- ✔️ Bleed line detection on both edges
- ✔️ Serial number character validation
- ✔️ Scrollable Tkinter-based result GUI
- ✔️ Modular & explainable pipeline

---

## 🛠️ Technologies Used

- **Python 3**
- **OpenCV**
- **NumPy**
- **Tkinter**
- **PIL (Pillow)**
- **Matplotlib**
- **Scikit-image (SSIM)**
- **CNN (Extensible / Training-ready module)**

---

## 🧩 System Architecture

```

Input Currency Image
↓
Preprocessing (Resize, Noise Removal, Grayscale)
↓
CNN-Based Classification (Real / Fake) [Optional / Extensible]
↓
Feature-Level Verification (10 Features)
├── ORB + SSIM (Features 1–7)
├── Bleed Line Detection (Features 8–9)
└── Serial Number Analysis (Feature 10)
↓
Rule-Based Decision Engine
↓
Result Visualization via GUI

```

---

## 🔍 Currency Security Features Analyzed

| Feature No. | Security Feature |
|------------|------------------|
| 1–7 | Structural pattern similarity using ORB + SSIM |
| 8 | Left-side bleed line detection |
| 9 | Right-side bleed line detection |
| 10 | Serial number character count verification |

---

## 📊 Decision Logic

- Each feature returns **PASS** or **FAIL**
- Final result is calculated as:

```

X / 10 features PASSED

````

- Higher pass count → Higher authenticity confidence
- CNN output (if enabled) strengthens final classification

---

## 🖥️ Graphical User Interface (GUI)

### 1️⃣ Starting GUI
- Select input currency image
- Choose currency denomination
- Submit image for analysis

### 2️⃣ Ending GUI
- Displays:
  - Original input image
  - Feature-wise processed images
  - SSIM scores and statistics
  - PASS / FAIL status for each feature
  - Final authenticity summary
- Scroll-enabled layout for better visualization

---

## ▶️ How to Run the Project

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/fake-currency-detection-cnn.git
cd fake-currency-detection-cnn
````

### 2️⃣ Install Dependencies

```bash
pip install opencv-python numpy pillow matplotlib scikit-image
```

> Optional (for CNN extension):

```bash
pip install tensorflow keras
```

### 3️⃣ Run the Application

```bash
python main.py
```

---

## 📁 Project Structure

```
├── Dataset/
│   └── 500_Features_Dataset/
├── gui_start.py
├── preprocessing.py
├── cnn_model.py            # (Optional / Extensible)
├── feature_extraction.py
├── decision_engine.py
├── gui_result.py
├── main.py
├── requirements.txt
└── README.md
```

---

## 🧪 CNN Module (Design Note)

* CNN is designed to:

  * Classify notes as **Genuine / Fake**
  * Learn discriminative visual patterns
* Can be trained using:

  * Labeled real & fake currency images
* CNN output is intended to **augment** rule-based decisions

> This hybrid design ensures **accuracy + explainability**, making it suitable for academic and research use.

---

## 🎓 Academic & Research Relevance

* Suitable for:

  * Final Year Project
  * Computer Vision / AI Mini Project
  * IEEE Conference Paper
* Demonstrates:

  * Hybrid AI system design
  * Explainable AI concepts
  * Feature-based verification
  * GUI-driven ML application

---

## 🚀 Future Enhancements

* Full CNN model training and integration
* Multi-denomination support (₹100, ₹200, ₹2000)
* Real-time camera input
* Web or mobile application
* Dataset expansion and augmentation

---




---



