# 🐱🐶 Cats vs Dogs Image Classification using CNN

A hands-on deep learning project that uses a **Convolutional Neural Network (CNN)** to classify images as either **Cat 🐱** or **Dog 🐶**.

The project is built using **Python, TensorFlow, and Keras** and covers the complete machine-learning workflow — from exploring and preprocessing raw images to training, evaluating, saving, and testing the trained CNN on completely new images.

---

## 📌 Project Overview

This project implements a **Convolutional Neural Network (CNN)** for binary image classification.

The model is trained using labeled images of cats and dogs. After training, the saved model can be used to predict the class of an image it has never seen during training or evaluation.

The project is organized into two main Jupyter notebooks:

1. **`Cat_dog_Model.ipynb`** — Contains the complete model development workflow, including data exploration, preprocessing, CNN construction, training, validation, evaluation, and model saving.
2. **`Test_Cat_Dog_Model.ipynb`** — Loads the saved model and tests it on **new images that are separate from both the training and test datasets**.

---

## 🎯 Project Objectives

* Import and organize the Cats vs Dogs dataset
* Explore and visualize the image dataset
* Understand image dimensions and class distribution
* Preprocess images for CNN training
* Build a Convolutional Neural Network
* Train and validate the model
* Evaluate the trained model
* Visualize training and validation accuracy
* Visualize training and validation loss
* Generate a confusion matrix
* Generate a classification report
* Save the trained CNN model
* Load the saved model independently
* Test the model on completely new/unseen images
* Display the predicted class and confidence
* Understand the complete image-classification pipeline
* Explore techniques for improving model performance

---

## 📂 Project Structure

```text
cats-dogs-cnn/
│
├── data/
│   └── raw/
│       ├── training_set/
│       │   ├── cats/
│       │   └── dogs/
│       │
│       ├── test_set/
│       │   ├── cats/
│       │   └── dogs/
│       │
│       └── new_images/
│           ├── cat.jpg
│           ├── dog.jpg
│           └── ...
│
├── notebooks/
│   ├── Cat_dog_Model.ipynb
│   └── Test_Cat_Dog_Model.ipynb
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

### 📁 Directory Explanation

| Directory/File                       | Purpose                                                        |
| ------------------------------------ | -------------------------------------------------------------- |
| `data/raw/training_set/`             | Images used for training the CNN                               |
| `data/raw/test_set/`                 | Images used for evaluating the trained model                   |
| `data/raw/new_images/`               | Completely new images used for independent prediction testing  |
| `notebooks/Cat_dog_Model.ipynb`      | Main notebook containing the complete CNN development workflow |
| `notebooks/Test_Cat_Dog_Model.ipynb` | Testing notebook for predicting completely new images          |
| `models/`                            | Stores the trained CNN model                                   |
| `reports/figures/`                   | Stores generated graphs and visualizations                     |
| `requirements.txt`                   | Python dependencies required to run the project                |
| `README.md`                          | Project documentation                                          |

---

# 📓 Jupyter Notebooks

## 1. 🧠 `Cat_dog_Model.ipynb`

This is the **main structured notebook** of the project.

It contains the complete workflow for developing the Cats vs Dogs CNN model:

```text
Dataset
   ↓
Data Exploration
   ↓
Image Preprocessing
   ↓
Train/Validation Preparation
   ↓
CNN Architecture
   ↓
Model Compilation
   ↓
Model Training
   ↓
Validation
   ↓
Model Evaluation
   ↓
Performance Visualization
   ↓
Model Saving
```

The notebook is organized into clear sections so that each stage of the CNN pipeline can be understood independently.

### Main Sections

* Project setup
* Importing libraries
* Dataset exploration
* Class distribution
* Image visualization
* Image preprocessing
* Training and validation preparation
* CNN architecture
* Model compilation
* Model training
* Training history
* Accuracy visualization
* Loss visualization
* Test-set evaluation
* Confusion matrix
* Classification report
* Saving the trained model

---

## 2. 🔍 `Test_Cat_Dog_Model.ipynb`

This notebook is designed specifically for **testing the saved CNN model on new images**.

It is separate from the training notebook so that the trained model can be tested independently.

The images used in this notebook are stored in:

```text
data/raw/new_images/
```

These images should **not be part of the original training or test dataset**.

### Testing Workflow

```text
Saved CNN Model
       ↓
Select New Image
       ↓
Display Image
       ↓
Resize to 256 × 256
       ↓
Normalize Pixel Values
       ↓
Add Batch Dimension
       ↓
CNN Prediction
       ↓
Cat 🐱 / Dog 🐶
       ↓
Confidence Score
       ↓
Display Result
```

The testing notebook currently selects a **random image** from the `new_images` directory whenever the image-selection cell is executed.

This provides an easy way to repeatedly test the trained model on different unseen images.

---

# 🧠 CNN Architecture

The model uses a **Convolutional Neural Network** to automatically learn visual features from the images.

The general architecture follows:

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

Convolutional layers learn visual patterns such as edges, textures, shapes, and increasingly complex features as the network becomes deeper.

---

# 🛠️ Technologies Used

* **Python**
* **TensorFlow**
* **Keras**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Scikit-learn**
* **Pillow**

---

# ⚙️ Installation

## 1. Clone the Repository

```bash
git clone <your-repository-url>
```

## 2. Navigate to the Project

```bash
cd cats-dogs-cnn
```

## 3. Create a Virtual Environment

```bash
python -m venv .venv
```

## 4. Activate the Virtual Environment

### Windows

```bash
.venv\Scripts\activate
```

### Linux / macOS

```bash
source .venv/bin/activate
```

## 5. Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 📊 Dataset

The project contains two primary classes:

* 🐱 **Cats**
* 🐶 **Dogs**

The original dataset is divided into:

### Training Set

```text
data/raw/training_set/
├── cats/
└── dogs/
```

The training images are used to teach the CNN how to distinguish between cats and dogs.

### Test Set

```text
data/raw/test_set/
├── cats/
└── dogs/
```

The test images are used to evaluate how well the trained model performs on images that were not used during training.

---

# 🆕 Testing on Completely New Images

An additional directory is provided for testing the saved model on images outside the original dataset:

```text
data/raw/new_images/
```

For example:

```text
data/
└── raw/
    └── new_images/
        ├── cat.jpg
        ├── dog.jpg
        └── another_image.png
```

These images are intended to be **independent of both the training and test sets**.

The `Test_Cat_Dog_Model.ipynb` notebook randomly selects one of these images, preprocesses it using the same image-processing procedure used by the model, and sends it to the saved CNN.

The prediction includes:

```text
Predicted class: Cat
Confidence: 91.27%
```

or:

```text
Predicted class: Dog
Confidence: 84.63%
```

> **Note:** The confidence score represents the model's output probability and should not be interpreted as a guarantee that the prediction is correct.

---

# 🚀 Complete Project Workflow

```text
                    DATASET
                       │
                       ▼
              Data Exploration
                       │
                       ▼
             Image Preprocessing
                       │
                       ▼
              CNN Model Building
                       │
                       ▼
                Model Training
                       │
                       ▼
                  Validation
                       │
                       ▼
               Model Evaluation
                       │
             ┌─────────┴─────────┐
             ▼                   ▼
       Visualization        Save Model
                                 │
                                 ▼
                         New Unseen Images
                                 │
                                 ▼
                         Independent Testing
                                 │
                                 ▼
                          Cat 🐱 / Dog 🐶
```

---

# 📈 Model Evaluation

The trained CNN is evaluated using several performance metrics and visualizations.

### Evaluation Metrics

* **Accuracy**
* **Loss**
* **Confusion Matrix**
* **Classification Report**

### Visualizations

* Training Accuracy
* Validation Accuracy
* Training Loss
* Validation Loss
* Confusion Matrix
* Sample image predictions

These evaluations help determine how effectively the CNN learns and generalizes to unseen data.

---

# 💾 Model Saving

After training and evaluation, the trained model is saved inside the `models/` directory.

```text
models/
└── trained_model.keras
```

The saved model can then be loaded independently by:

```text
Test_Cat_Dog_Model.ipynb
```

This means the model does **not need to be retrained every time a new image is tested**.

---

# 🔮 Future Improvements

The model can be improved using several deep-learning techniques:

* Data Augmentation
* Dropout layers
* Batch Normalization
* Hyperparameter tuning
* Learning-rate optimization
* Transfer Learning
* Pretrained **VGG16**
* Pretrained **ResNet**
* Pretrained **MobileNet**
* Increasing dataset size
* Improving image preprocessing
* Model deployment as a web application
* Creating an interactive image-prediction interface

---

# 👨‍💻 Author

**Suraj Chalise**

---

# 📚 Learning Goal

This project is created as a **hands-on learning project** to develop a practical understanding of Convolutional Neural Networks and image classification.

The goal is to understand the complete pipeline:

```text
Raw Images
    ↓
Data Exploration
    ↓
Preprocessing
    ↓
CNN
    ↓
Training
    ↓
Validation
    ↓
Evaluation
    ↓
Model Saving
    ↓
New Image
    ↓
Prediction
```

Rather than only training a model, the project demonstrates how a trained CNN can be **saved, loaded, and independently tested on completely new images**.

This makes the project useful for understanding both the **development** and **practical application** of a CNN-based image classification system.
