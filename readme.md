# 🎙 Speech Emotion Recognition and Intensity Prediction using CREMA-D

## 📌 Overview

This project implements Speech Emotion Recognition (SER) and Emotion Intensity Prediction using the CREMA-D dataset.

Two approaches were explored:

1️⃣ Classical Machine Learning using MFCC + Ensemble Methods  
2️⃣ Deep Learning using Fine-Tuned Wav2Vec 2.0 (Multi-task Learning)

---

## 📂 Dataset

Dataset used: CREMA-D (Crowd-Sourced Emotional Multimodal Actors Dataset)
https://www.kaggle.com/datasets/ejlok1/cremad?resource=download

- 7442 audio samples
- 6 emotion classes:
  - Angry
  - Happy
  - Sad
  - Fear
  - Disgust
  - Neutral
- 3 intensity levels:
  - Low
  - Medium
  - High

---

## 🧠 Approach 1: Classical ML (MFCC + Ensemble)

### Pipeline:
- Audio preprocessing (3 sec clips)
- MFCC feature extraction
- Feature scaling
- Random Forest / Ensemble classifier
- Random Forest Regressor for intensity

### Results:
- Emotion Classification Accuracy: ~50%
- Intensity MAE: ~0.17

---

## 🚀 Approach 2: Wav2Vec 2.0 Fine-Tuning

Model Used:
- facebook/wav2vec2-base (HuggingFace Transformers)

Architecture:
- Pretrained Wav2Vec2 encoder
- Classification head (Emotion)
- Regression head (Intensity)

### Results:
- Emotion Accuracy: 75% 
- Intensity MAE: 0.17

---

## ⚙️ Installation

1. Clone repository: Upload repo in Drive(for Collab)

2. Install dependencies: pip install -r requirements.txt

3. Download and upload Creama-D Dataset in Drive

---

## ▶ How to Run

### Option 1 – Classical ML
Open: Emotion Recognition & Prediction(Classic ML).ipynb

Run all cells sequentially.

---

### Option 2 – Wav2Vec 2.0
Open: Emotion & intensity prediciton (Pretrained CNN).ipynb

Enable GPU before running.

---




