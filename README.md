# Skin Cancer Classification using CNN

This project focuses on automated skin lesion classification using deep learning. The goal is to classify skin cancer types from dermoscopic images using a Convolutional Neural Network (CNN). The dataset used is HAM10000 — a widely used medical dataset containing 10,015 skin lesion images across 7 different cancer classes.

---

## 🚀 Project Objectives

- To apply deep learning for medical image classification
- To develop a CNN model for 7-class skin lesion classification
- To better understand dataset distribution, image imbalance, and feature variations through EDA
- To train a baseline CNN model with data augmentation
- To evaluate performance using accuracy and loss metrics

---



## 📊 Dataset: HAM10000

Seven different disease classes are included:

| Class | Full Form | Type |
|-------|-----------|------|
| AKIEC | Actinic Keratoses | precancerous |
| BCC   | Basal Cell Carcinoma | cancer |
| BKL   | Benign Keratosis | benign |
| DF    | Dermatofibroma | benign |
| MEL   | Melanoma | cancer |
| NV    | Melanocytic Nevi | benign |
| VASC  | Vascular Lesions | benign/malignant |

---

## 🔍 EDA (Exploratory Data Analysis)

Performed in `EDA.ipynb`:

- Class distribution visualization
- Image shape and resolution analysis
- Lesion color & texture variation
- Dataset imbalance identification
- Example image preview for each class

Key findings:

- Dataset is highly imbalanced
- NV class dominates most samples
- MEL (Melanoma) — the deadliest form — is underrepresented  
  → requires class balancing / augmentation for best results

---

## 🧠 Model Development (CNN)

Implemented in `base_modelCNN.ipynb`.

### Model Features:

- Input shape: `64 x 64 x 3`
- Convolutional layers for feature extraction
- Batch normalization
- Max pooling
- Dropout to reduce overfitting
- Fully connected classification head
- Softmax output for 7 classes

---

## 🧪 Training Setup

- Optimizer: Adam  
- Loss: Categorical crossentropy  
- Train/validation split  
- Metric: Accuracy  
- Data augmentation applied:
  - rotation
  - zoom
  - horizontal flip
  - shift

---

## 📈 Results & Evaluation

Tracked:

- Training accuracy
- Validation accuracy
- Training vs validation loss
- Overfitting trend monitoring

The model shows improving generalization as epochs increase, and validation accuracy gradually converges.

---

## 🧑‍⚕️ Real-World Use Cases

- Early melanoma cancer detection
- Dermatology decision support
- Telemedicine & remote screening system
- AI-assisted diagnosis tools

⚠️ Note:  
This is a research/experimental system — not a certified diagnostic tool.

---

## 🏆 Key Takeaways

- Learned medical imaging preprocessing  
- Experience working with imbalanced datasets  
- Implemented CNN from scratch  
- Performed meaningful EDA on real medical dataset  
- Understood challenges in cancer classification modeling  

---


