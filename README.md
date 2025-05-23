**Pneumonia Detection from Chest X-Rays**

**📌 Project Overview**
A deep learning-based diagnostic system that classifies chest X-ray images into Normal or Pneumonia cases using a fine-tuned VGG16 model with transfer learning. The model achieves high accuracy and reliability, making it suitable for assisting medical diagnosis.
__________________________________________________________________________________________
** Dataset**
Source: [Chest X-Ray Images (Pneumonia) | Kaggle
](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
Classes: Normal (1,349 images) | Pneumonia (3,883 images)

Split: Train (70%) | Validation (15%) | Test (15%)
_______________________________________________________________________________________
**Model Architecture**
Base Model:
VGG16 (pretrained on ImageNet, include_top=False)

Input Shape: (224, 224, 3)

Custom Classification Head:
Global Average Pooling

Dense Layer (128 units, ReLU activation)

Output Layer (1 unit, Sigmoid activation)
_______________________________________________________________________________________
**Training Configuration:**
Optimizer: Adam (lr=0.0001)

Loss: Binary Crossentropy

Metrics: Accuracy, Precision, Recall

Callbacks: Early Stopping, Model Checkpointing
_______________________________________________________________________________________
📈 Performance Metrics
Metric	Training	Validation	Test
Accuracy, Precision, Recall, F1-Score	
_______________________________________________________________________________________
**Tools & Technologies**
Languages: Python 3.x

Libraries: TensorFlow, Keras, OpenCV, NumPy, Matplotlib, scikit-learn

Data Handling: OpenDatasets (Kaggle integration)

![Image](https://github.com/user-attachments/assets/d840657a-a7bd-4552-95c6-c9ab1d3c432b)
