# Guava Disease Detection using Deep Learning

## 📌 Overview

This project focuses on **automated detection of guava diseases** using deep learning models. It evaluates multiple architectures across **two different datasets** to analyze performance, robustness, and generalization.

The study includes:

* Classical CNN architectures
* Modern pretrained deep networks
* Transformer-based models

A key aspect of this work is **cross-dataset evaluation**, ensuring models are not only accurate but also generalize well.

---

## 📂 Project Structure

```
├── Dataset_1/        # Primary dataset (fruit images)
├── Dataset_2/        # Benchmark dataset (filtered: fruits only)
├── Models/
│   ├── Dataset_1_Models/
│   ├── Dataset_2_Models/
└── README.md
```

---

## 📊 Datasets

### 🔹 Dataset 1 — Guava Fruit Disease Dataset

**Source:** Mendeley Data

**Classes:**

* Anthracnose
* Fruit Flies
* Healthy Fruits

**Details:**

* Original: 473 images
* Augmented: 3,784 images
* Image Size: 512 × 512 (RGB)
* Location: Bangladesh (Rajshahi & Pabna)
* Verified by plant pathologists

📎 Link: https://data.mendeley.com/datasets/bkdkc4n835/1

---

### 🔹 Dataset 2 — Guava Leaves & Fruits Dataset (Filtered)

**Source:** Mendeley Data

⚠️ **Important Modification:**
For this study, Dataset 2 was **filtered to include only fruit images**. All **leaf-based classes were excluded** to maintain consistency with Dataset 1 and ensure fair comparison.

**Included Classes (Fruits Only):**

* Phytophthora
* Scab
* Styler and Root

**Excluded Classes:**

* ❌ Red Rust (leaf-based disease)
* ❌ Disease-free leaves

**Details:**

* Original: 527 images
* Augmented: 4,899 images
* Image Size: 512 × 512
* Source: Bangladesh Agricultural University

📎 Link: https://data.mendeley.com/datasets/x84p2g3k6z/1

---

## 🧠 Models Implemented

### 🔸 Models Used on **Both Datasets**

The following CNN and pretrained architectures were trained and evaluated on **both Dataset 1 and filtered Dataset 2**:

* Custom CNN
* AlexNet
* VGG16
* ResNet50
* EfficientNet-B0
* InceptionV3

---

### 🔸 Transformer Models

#### 📍 Dataset 1:

* Vision Transformer (ViT)
* DeiT (Data-efficient Image Transformer)
* Swin Transformer

#### 📍 Dataset 2:

* DeiT (only transformer used)

---

## 📈 Results

* Accuracy
* Loss curves
* Confusion matrices

---

## 🚀 Future Work

* Include real-time mobile deployment
* Expand dataset with more field conditions
* Explore lightweight models for edge devices

---

## 📜 License

This project is for academic and research purposes.
