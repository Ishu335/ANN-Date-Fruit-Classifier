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

**Class** → Type of Date Fruit

The dataset contains **7 different classes of date fruits**.

---

## 🧠 ANN Model Architecture

The Artificial Neural Network used in this project has the following structure:

```
Input Layer        : 32 Features
Hidden Layer 1     : 62 Neurons (ReLU)
Hidden Layer 2     : 62 Neurons (ReLU)
Output Layer       : 7 Neurons (Softmax)
```

### Explanation

- **Input Layer (32 neurons)**  
  Represents the 32 numerical features extracted from the dataset.

- **Hidden Layers (62 neurons each)**  
  Two fully connected layers learn complex patterns from the input features.

- **Activation Function**
  - **ReLU** is used in hidden layers
  - **Softmax** is used in the output layer for **multi-class classification**

- **Output Layer (7 neurons)**  
  Each neuron represents one **date fruit class**.

---

## ⚙️ Technologies Used

- Python
- PyTorch
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## 📈 Training Visualization

Training and validation losses are tracked during model training.

```python
import matplotlib.pyplot as plt

plt.plot(epoch_train_loss, label="Training Loss")
plt.plot(epoch_val_loss, label="Validation Loss")
plt.xlabel("Epoch")
plt.ylabel("Loss")
plt.title("Training vs Validation Loss")
plt.legend()
plt.show()
```

---

## 🎯 Results

The ANN model successfully learns patterns in the dataset and performs **multi-class classification** of date fruit types based on morphological and texture features.

---

## 🔮 Future Improvements

- Hyperparameter tuning
- Adding Dropout layers
- Model optimization
- Deploying the model as an API

---

## 👨‍💻 Author

**Ishwar Sonawane**

Machine Learning Enthusiast | Python Developer
