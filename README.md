# 🐶🐱 Dog vs Cat Classification with Custom CNN

This project is a binary image classification model that distinguishes between **cats** and **dogs** using a **custom-built Convolutional Neural Network (CNN)** in TensorFlow/Keras.

## 📁 Dataset

For this used the [Microsoft Dogs vs Cats Dataset](https://www.kaggle.com/datasets/microsoft/catsvsdogs), available on Kaggle, which contains 25,000 labeled images of cats and dogs.

## 🧠 Model Architecture

The CNN model consists of:

- 4 convolutional layers with increasing filters (32 → 256)
- Batch Normalization after each convolution
- MaxPooling after each convolution
- Dropout layer before the dense layer to prevent overfitting
- Final Dense layer with sigmoid activation for binary classification

### Loss & Optimization
- **Loss Function**: Binary Crossentropy  
- **Optimizer**: Adam  
- **Evaluation Metric**: Accuracy

## 🧪 Evaluation

Model performance was evaluated using:

- **Accuracy**
- **Classification Report** (Precision, Recall, F1-score)
- **Confusion Matrix**
- Visualizations on random test images

The final model achieved reasonable accuracy on unseen validation images, with prediction visualizations for both correct and incorrect classifications.

## 📊 Sample Output

| Prediction | True Label | Result |
|------------|------------|--------|
| Dog        | Dog        | ✅     |
| Cat        | Dog        | ❌     |

<![Image](https://github.com/user-attachments/assets/214c9163-650c-4f67-b25a-2b11d40f51c0) width="600"/>
