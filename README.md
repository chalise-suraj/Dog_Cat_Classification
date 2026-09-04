# 🐱🐶 Cats vs Dogs Image Classification using CNN

## 📌 Project Overview

This project implements a **Convolutional Neural Network (CNN)** to classify images of **cats and dogs**.

The model is built using **TensorFlow and Keras** and trained on labeled images. Given a new image, the trained model predicts whether the image contains a **Cat 🐱** or a **Dog 🐶**.

---

## 🎯 Project Objectives

* Import and organize the Cats vs Dogs dataset
* Explore and visualize image data
* Preprocess images for CNN training
* Build a Convolutional Neural Network
* Train and validate the model
* Evaluate model performance
* Visualize accuracy and loss
* Make predictions on new images
* Improve performance using techniques such as data augmentation

---

## 📂 Project Structure

```text
cats-dogs-cnn/
│
├── data/
│   ├── training_set/
│   │   ├── cats/
│   │   └── dogs/
│   │
│   └── test_set/
│       ├── cats/
│       └── dogs/
│
├── notebooks/
│   └── cats_dogs_cnn.ipynb
│
├── models/
│   └── trained_model.keras
│
├── reports/
│   └── figures/
│
├── requirements.txt
│
└── README.md
```

---

## 🛠️ Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* Pillow

---

## 🧠 CNN Architecture

The model will use Convolutional Neural Network layers to automatically learn important features from images.

```text
Input Image
     ↓
Convolution Layer
     ↓
ReLU Activation
     ↓
Max Pooling
     ↓
Convolution Layer
     ↓
ReLU Activation
     ↓
Max Pooling
     ↓
Flatten
     ↓
Dense Layer
     ↓
Output Layer
     ↓
Cat 🐱 / Dog 🐶
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone <your-repository-url>
```

Navigate to the project directory:

```bash
cd cats-dogs-cnn
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate the virtual environment.

### Windows

```bash
.venv\Scripts\activate
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

---

## 📊 Dataset

The dataset contains images of two classes:

* 🐱 Cats
* 🐶 Dogs

The dataset is divided into:

* **Training Set** — Used to train the CNN
* **Test Set** — Used to evaluate the trained model

---

## 🚀 Project Workflow

```text
Dataset
   ↓
Data Exploration
   ↓
Image Preprocessing
   ↓
CNN Model Building
   ↓
Model Training
   ↓
Validation
   ↓
Model Evaluation
   ↓
Predictions
```

---

## 📈 Evaluation

The model will be evaluated using:

* Accuracy
* Loss
* Confusion Matrix
* Classification Report

Training and validation performance will also be visualized using graphs.

---

## 🔮 Future Improvements

Possible improvements include:

* Data Augmentation
* Dropout layers to reduce overfitting
* Batch Normalization
* Transfer Learning
* Using pretrained models such as VGG16, ResNet, or MobileNet
* Hyperparameter tuning
* Deploying the model as a web application

---

## 👨‍💻 Author

**Suraj Chalise**

---

## 📚 Learning Goal

This project is created as a hands-on learning project to deeply understand how **Convolutional Neural Networks (CNNs)** work for image classification, from raw image data to a trained deep learning model.
