# 🐶🐱 Dog vs Cat Classification with Custom CNN

This project is a binary image classification model that distinguishes between **cats** and **dogs** using a **custom-built Convolutional Neural Network (CNN)** in TensorFlow/Keras.

## 📁 Dataset

For this used the [Microsoft Dogs vs Cats Dataset](https://www.kaggle.com/datasets/microsoft/catsvsdogs), available on Kaggle, which contains 25,000 labeled images of cats and dogs.
```bash
https://www.kaggle.com/datasets/microsoft/catsvsdogs
```
- Preprocessing:
  - Corrupt images removed
  - Normalized and resized to 224x224
  - Data augmentation applied (rotation, zoom, flip, shift, etc.)

---
## 🧠 Model Overview

- **Type**: Binary Image Classification (Cat = 0, Dog = 1)
- **Framework**: TensorFlow/Keras
- **Architecture**:
  - 4 Convolutional layers
  - Batch Normalization after each conv layer
  - MaxPooling layers
  - Dropout before the dense layers
  - Final sigmoid activation

- **Loss**: Binary Crossentropy  
- **Optimizer**: Adam  
- **Input Size**: 224x224 RGB Images  

---

## 📊 Evaluation Results (on Validation Set)

| Metric     | Cat (0)  | Dog (1)  |
|------------|----------|----------|
| Precision  | 0.85964  | 0.95723  |
| Recall     | 0.96242  | 0.84261  |
| F1-score   | 0.90813  | 0.89627  |
| Support    | 2501     | 2497     |

- **Accuracy**: 90.26%  
- **Macro Avg F1-score**: 90.22%  
- **Weighted Avg F1-score**: 90.22%

✅ The model shows high performance with balanced precision and recall for both classes.

---

## Sample Predictions

![Image](https://github.com/user-attachments/assets/214c9163-650c-4f67-b25a-2b11d40f51c0) 
