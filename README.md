# MRI_tumor_detection_CNN
MRI based brain tumor detection using CNN
This project leverages a Convolutional Neural Network (CNN) to classify brain MRI images into two categories for brain tumor detection. The dataset used is sourced from Kaggle, and the model achieves over 82% accuracy on the test set.

---

## Project Goals
The primary objective of this project is to:
- Develop a robust CNN model for classifying brain MRI images.
- Achieve high accuracy in distinguishing images into tumor and non-tumor categories.
- Implement image augmentation and preprocessing to enhance model performance.
  
---

## Dataset
- **Source**: [Brain MRI Images for Brain Tumor Detection on Kaggle](https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection)
- **Description**: The dataset consists of brain MRI images categorized into two classes.
- **Structure**:
  - brain_tumor_dataset
    - no (98 images)
    - yes (155 images)
![dataset](https://github.com/user-attachments/assets/8627c372-80dc-4beb-99db-3fd08c797909)

---

## Model Architecture
The Convolutional Neural Network (CNN) architecture comprises:
1. **Input Layer**: Images resized to 256x256x3.
2. **Preprocessing Layers**:
 - Rescaling pixel values to [0,1].
 - Data augmentation (random flipping and rotation).
3. **Convolutional and Pooling Layers**:
 - Six convolutional layers with ReLU activation and max-pooling.
4. **Dense Layers**:
 - Fully connected layers with ReLU and Softmax activation for classification.
5. **Output Layer**: Predicts one of the two classes.

---


## Training
-Epochs: 30
-Batch Size: 23
-Optimizer: Adam
-Loss Function: Sparse Categorical Crossentropy
![accuracy chart](https://github.com/user-attachments/assets/93fc4bde-d875-4453-9fd9-2c96d2d4a1e8)
![loss chart](https://github.com/user-attachments/assets/05eb16a2-b688-4369-a452-e156b0c6ea1a)

---

## Results
-Training Accuracy: 86.97%
-Validation Accuracy: 91.30%
-Test Accuracy: 82.06%
 
The model demonstrates effective classification with good generalization across unseen data.

![result](https://github.com/user-attachments/assets/32c2ec72-c270-4b20-aa36-fee0beb57038)

