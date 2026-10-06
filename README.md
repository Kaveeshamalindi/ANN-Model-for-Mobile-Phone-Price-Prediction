# ANN-Model-for-Mobile-Phone-Price-Prediction

This project demonstrates how to build and train a simple **Artificial Neural Network (ANN)** model using **TensorFlow** to classify mobile phones into two price ranges:

* `0` → Low Price
* `1` → High Price

The model learns the relationship between mobile phone specifications such as RAM, internal memory, battery power, and other features and the corresponding price range.

This task was completed using **Google Colab**.

---

## 🎯 Objective

The main objective of this task is to develop a small ANN model that can predict whether a mobile phone belongs to the **low-price** or **high-price** category based on its specifications.

The trained model weights are also saved for future predictions.

---

## 📂 Dataset

The dataset is provided as a CSV file:

```text
mobile_price.csv
```

The dataset contains different mobile phone specifications and a target column representing the price range.

### Target Classes

| Value | Price Range |
| ----: | ----------- |
|     0 | Low         |
|     1 | High        |

---

## 🛠️ Technologies Used

* Python
* Google Colab
* TensorFlow / Keras
* Pandas
* Scikit-learn

---

## 🧠 ANN Architecture

The ANN consists of two hidden layers as required by the task.

```text
Input Features
       ↓
Dense Layer
8 Neurons
ReLU Activation
       ↓
Dense Layer
4 Neurons
ReLU Activation
       ↓
Output Layer
1 Neuron
Sigmoid Activation
       ↓
Low (0) / High (1)
```

### Model Configuration

| Component         | Configuration       |
| ----------------- | ------------------- |
| Hidden Layer 1    | 8 neurons           |
| Hidden Layer 2    | 4 neurons           |
| Activation        | ReLU                |
| Output Layer      | 1 neuron            |
| Output Activation | Sigmoid             |
| Optimizer         | Adam                |
| Loss Function     | Binary Crossentropy |
| Training Epochs   | 100                 |
| Batch Size        | 32                  |
| Training Data     | 75%                 |
| Testing Data      | 25%                 |

---

## 📊 Results

After training, the model is evaluated using the testing dataset.

Add your final result below after running the model:

```text
Test Loss: 0.32206135988235474
Test Accuracy: 0.8659999966621399
```

---

## 💾 Saved Model Weights

The trained ANN weights are saved as:

```text
mobile_price_ann.weights.h5
```

These weights can later be loaded into the same ANN architecture to make predictions on new mobile phone specifications.

---

## 📚 Learning Outcomes

Through this task, I learned how to:

* Load a CSV dataset using Pandas
* Separate features and target values
* Split data into training and testing sets
* Perform feature scaling
* Build a simple ANN using TensorFlow/Keras
* Configure hidden layers and neurons
* Compile an ANN model
* Train a model using epochs and batch size
* Evaluate model performance
* Save trained model weights
