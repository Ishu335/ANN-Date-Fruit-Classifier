# Date Fruit Classification using Artificial Neural Networks (ANN)

## 📌 Project Overview
This project implements an **Artificial Neural Network (ANN)** to classify different types of **date fruits** using morphological features from the dataset.

The model learns complex relationships between fruit characteristics and predicts the correct **date fruit class** using a **multi-class classification approach**.

This project demonstrates the application of **Deep Learning in agricultural data analysis and product classification.**

---

## 📊 Dataset

The dataset contains features extracted from date fruit images.

### Features

- AREA
- PERIMETER
- MAJOR_AXIS
- MINOR_AXIS
- ECCENTRICITY
- EQDIASQ
- SOLIDITY
- CONVEX_AREA
- EXTENT
- ASPECT_RATIO
- ROUNDNESS
- COMPACTNESS
- SHAPEFACTOR_1
- SHAPEFACTOR_2
- SHAPEFACTOR_3
- SHAPEFACTOR_4
- Texture-based features

### Target Variable

**Class → Type of Date Fruit**

The dataset contains **7 different classes of date fruits**.

---

# 🧠 ANN Model Architecture

The Artificial Neural Network used in this project has the following structure:


---

## 🏗 Architecture Diagram

### ANN Architecture Visualization

![ANN Architecture](https://github.com/Ishu335/ANN-Date-Fruit-Classifier/blob/4167b7f5546c10a747ed05b5e85dffbc981d131e/Architecture%20Image/ChatGPT%20Image%20Mar%208%2C%202026%2C%2006_51_43%20PM.png)

![ANN Architecture](https://github.com/Ishu335/ANN-Date-Fruit-Classifier/blob/4167b7f5546c10a747ed05b5e85dffbc981d131e/Architecture%20Image/ChatGPT%20Image%20Mar%208%2C%202026%2C%2006_51_58%20PM.png)

---

## 🧩 Model Explanation

- **Input Layer (32 neurons)**  
  Represents the 32 numerical features extracted from the dataset.

- **Hidden Layer 1 (62 neurons)**  
  A fully connected layer followed by **ReLU activation** to introduce non-linearity.

- **Hidden Layer 2 (62 neurons)**  
  Another dense layer that learns deeper feature representations.

- **Output Layer (7 neurons)**  
  Produces logits for **7 date fruit classes**.

⚠️ **Note:**  
Softmax is **not applied in the model** because **PyTorch's `CrossEntropyLoss` already applies LogSoftmax internally.**

---

## ⚙️ Technologies Used

- Python
- PyTorch
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---


