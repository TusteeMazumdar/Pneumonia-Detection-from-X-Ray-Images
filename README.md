**Pneumonia Detection from Chest X-Rays**

**📌 Project Overview**
A deep learning-based diagnostic system that classifies chest X-ray images into Normal or Pneumonia cases using a fine-tuned VGG16 model with transfer learning. The model achieves high accuracy and reliability, making it suitable for assisting medical diagnosis.

**Technical Implementation**
📂 Dataset
Source:(https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
Classes: Normal (1,349) | Pneumonia (3,883)

**Preprocessing**
Resizing (224×224)
Normalization (0-1 scaling)
Data Augmentation (rotation, shifts, zoom, flip)

**Model Architecture**
Base Model: VGG16 (pre-trained on ImageNet)
Fine-tuning: Last 5 layers unfrozen
Global Average Pooling
Dense (128 neurons, ReLU)
Output (Sigmoid, binary classification)

- **Training Setup**
Optimizer: Adam (LR=0.0001)
Loss: Binary Cross-Entropy
Early Stopping (patience=10)
Learning Rate Scheduling (decay after 15 epochs)


Performance & Evaluation:
Precision, Recall, Accuracy, F1-Score
Confusion Matrix Analysis (TP, TN, FP, FN)


** Key Features**
✔ High Diagnostic Accuracy (~92%)
✔ Robust Data Augmentation (prevents overfitting)
✔ Model Interpretability (sample predictions + visualizations)
✔ Unseen Image Testing (supports real-world deployment)


![Image](https://github.com/user-attachments/assets/d840657a-a7bd-4552-95c6-c9ab1d3c432b)
