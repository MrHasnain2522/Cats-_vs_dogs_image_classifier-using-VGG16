# project title:
 Cats vs Dogs classifier using VGG16

# intro:
This project builds a deep learning model to classify images of cats and dogs using transfer learning with the VGG16 model pre-trained on ImageNet.
Transfer learning allows us to leverage powerful features learned from large-scale datasets and fine-tune the model for our specific binary classification task.

## 🚀 Features

- Uses pre-trained **VGG16** on **ImageNet** for feature extraction
- Custom top layers for binary classification
- Image data generators for preprocessing
- Training with real-time data augmentation
- Evaluation with accuracy metrics

## 🧠 Model Architecture

- Base Model: VGG16 (pre-trained, `include_top=False`)
- Added Layers:
  - GlobalAveragePooling2D
  - Dense(128, ReLU)
  - Dropout(0.5)
  - Dense(1, Sigmoid)
 
  ## 📁 Dataset

You can use the **Kaggle Dogs vs Cats** dataset:
- [Kaggle Dataset Link](https://www.kaggle.com/c/dogs-vs-cats/data)

## 📈 Results
Accuracy: ~90%+ on validation set

Fast convergence due to pre-trained weights

Visual results include training curves and prediction samples

 # # 📚 Requirements
TensorFlow / Keras

NumPy

Matplotlib

Scikit-learn
