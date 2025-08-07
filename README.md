# 🧠 Fashion MNIST Classification – CS770 Assignment 3

In this project, the Fashion MNIST dataset was used to classify grayscale images of clothing items into ten categories. The dataset consists of 60,000 training images and 10,000 testing images, each with a resolution of 28×28 pixels. A variety of deep learning models, including a shallow neural network and several convolutional neural networks were developed, trained, and evaluated. The primary objective was to build and assess these models individually while applying hyperparameter tuning techniques to improve performance. Accuracy was used as the main evaluation metric, and confusion matrices along with classification reports were generated to provide a detailed evaluation.

---

## 📊 Dataset

- **Fashion MNIST**
  - 60,000 training images
  - 10,000 test images
  - 28×28 grayscale images
  - 10 classes:  
    `T-shirt/top`, `Trouser`, `Pullover`, `Dress`, `Coat`, `Sandal`, `Shirt`, `Sneaker`, `Bag`, `Ankle boot`

---

## 🏗️ Models Implemented

| Model    | Description                                | Accuracy |
|----------|--------------------------------------------|----------|
| Model 1.1 | Shallow NN with SGD                       | 78.85%   |
| Model 1.2 | Shallow NN with Adam                      | 84.56%   |
| Model 1.3 | Shallow NN with SGD, larger batch size    | 80.57%   |
| Model 2.1 | Basic CNN with Adam                       | 87.01%   |
| Model 2.2 | CNN with RMSprop + Dropout                | 84.14%   |
| Model 2.3 | CNN with Adam + Dropout                   | 87.29%   |
| Model 3.1 | Deep CNN with 2 Conv2D layers             | 89.60%   |
| Model 3.2 | Deep CNN + Dropout                        | 90.16%   |
| Model 3.3 | Deep CNN + Dropout + lower LR             | **91.80%** |
| Extra Task | Custom NN with Concat + BN + Dropout     | 85.78%   |

---

## 📈 Experiments & Evaluation Metrics

- **Training Details**:
  - 10 epochs per model
  - Validation split from training set
  - Normalized grayscale inputs
  - One-hot encoded labels

- **Hyperparameters Explored**:
  - Optimizers: SGD, Adam, RMSprop
  - Learning rates and batch sizes
  - Dropout and Batch Normalization
  - Custom architecture with concatenation for extra task

- **Evaluation Metrics**:
  - ✅ Accuracy
  - ✅ Confusion Matrix
  - ✅ Precision, Recall, and F1 Score (per class)
  - ✅ Training and Validation curves
