# CNN-with-Min-Filter-for-Digit-Recognition

---

## 📊 Dataset Overview

- **Training Set:** 60,000 images  
- **Test Set:** 10,000 images  
- **Image Type:** Grayscale  
- **Image Dimensions:** 28 × 28 pixels  
- **Labels:** Digits 0 through 9

---

## 🧼 Min Filter for Image Denoising

The **Min Filter** is a non-linear image processing technique used to reduce **salt noise** (random white pixels) in images.

- **Function:** Replaces each pixel with the **minimum value** in its local neighborhood (e.g., 3×3 window).  
- **Effect:** Removes small bright spots while preserving darker image regions.

---

## 🧠 CNN Model Architecture

1. Input Layer: 28×28 grayscale image  
2. Convolutional Layer 1: 32 filters, 3×3 kernel, ReLU activation  
3. Max Pooling Layer 1: 2×2 pool size  
4. Convolutional Layer 2: 64 filters, 3×3 kernel, ReLU activation  
5. Max Pooling Layer 2: 2×2 pool size  
6. Flatten Layer  
7. Fully Connected Dense Layer: 128 units, ReLU activation  
8. Output Layer: 10 units (softmax activation for digits 0–9)

---

## 📈 Model Evaluation

- **Epochs:** 5  
- **Training Accuracy:** 94.89%  
- **Validation Accuracy:** 95.27%

---

## 🔍 Predictions

The model was tested on new digit images and achieved high prediction accuracy.  
It successfully recognized digits even with minor noise, demonstrating strong generalization.
