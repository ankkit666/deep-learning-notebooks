# Deep Learning Notebooks

A structured collection of hands-on notebooks covering core deep learning concepts — built from first principles through to modern training techniques, with every topic implemented in TensorFlow and Keras.

---

## About

This repository documents my deep learning practice journey as I transition from **7+ years in electrical power distribution (33/11KV systems, JVVNL, energy department at GoRajasthan)** into ML Engineering. Every concept is implemented from scratch in a dedicated notebook, with observations and notes written alongside the code.

**Focus areas:** Power systems · Smart grid analytics · Predictive maintenance · Load forecasting

---

## Topics Covered

### 1. Types of Neural Networks
- Artificial Neural Networks (ANN)
- Convolutional Neural Networks (CNN)
- Recurrent Neural Networks (RNN / LSTM / GRU)
- Autoencoders

### 2. Loss Functions
- Mean Squared Error (MSE) — regression
- Binary Cross-Entropy — binary classification
- Categorical Cross-Entropy — multi-class classification
- Comparison of loss functions across problem types

### 3. Backpropagation
- Chain rule — step-by-step derivation
- Forward pass vs backward pass
- Gradient computation in multi-layer networks
- Vanishing and exploding gradients

### 4. Gradient Descent
- Batch Gradient Descent
- Stochastic Gradient Descent (SGD)
- Mini-Batch Gradient Descent
- Learning rate effects — visualised on 2D datasets

### 5. Improving Neural Networks
- Train/validation/test split strategy
- Bias-variance tradeoff in deep networks
- Early stopping
- Learning curves — diagnosing overfitting vs underfitting

### 6. Activation Functions
- Sigmoid · Tanh · ReLU · Leaky ReLU · ELU
- Softmax for multi-class output
- Dead neuron problem in ReLU
- Choosing the right activation per layer

### 7. Weight Initialisation Techniques
- Zero initialisation — symmetry breaking failure
- Random initialisation
- Xavier / Glorot initialisation
- He initialisation
- Comparison on `ushape` and synthetic 2D datasets

### 8. Batch Normalisation
- Internal covariate shift — the problem it solves
- BatchNorm layer placement (before vs after activation)
- Effect on training speed and stability
- BatchNorm vs Dropout — when to use which

### 9. Optimizers
- SGD with momentum
- RMSprop
- Adam · AdaGrad · AdaDelta
- Side-by-side convergence comparison on the same model
- Choosing an optimizer for time-series energy data

### 10. Keras Tuner — Hyperparameter Optimisation
- RandomSearch tuner
- Hyperband tuner
- BayesianOptimization tuner
- Tuning: number of layers, units, learning rate, dropout rate
- Best practices for tuning deep learning models

---

## Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.10+ | Core language |
| TensorFlow 2.x | Deep learning framework |
| Keras (tf.keras) | Model building API |
| Scikit-learn | Preprocessing · Evaluation |
| NumPy · Pandas | Data manipulation |
| Matplotlib · Seaborn | Visualisation |
| Keras Tuner | Hyperparameter search |
| Jupyter / Google Colab | Notebook environment |

---

## Repository Structure

```
deep-learning-notebooks/
│
├── 01-types-of-neural-networks/
├── 02-loss-functions/
├── 03-backpropagation/
├── 04-gradient-descent/
├── 05-improving-neural-networks/
├── 06-activation-functions/
├── 07-weight-initialisation/
│   └── weight-init-ushape-xavier-he.ipynb
├── 08-batch-normalisation/
├── 09-optimizers/
├── 10-keras-tuner/
│
├── datasets/
│   └── X.csv
│
└── README.md
```

---

## How to Run

**Option 1 — Google Colab (recommended, no setup needed)**

Click the Colab badge inside any notebook folder.

**Option 2 — Local setup**

```bash
git clone https://github.com/ankkit666/deep-learning-notebooks.git
cd deep-learning-notebooks
pip install tensorflow keras scikit-learn pandas matplotlib seaborn keras-tuner
jupyter notebook
```

---

## Domain Application

Each concept is connected to a real-world energy sector use case wherever applicable:

| Deep Learning Concept | Energy Sector Application |
|---|---|
| LSTM / RNN | Hourly electricity demand forecasting |
| Autoencoder | Anomaly detection in distribution network load data |
| ANN Regression | Transformer loading prediction |
| Binary Classifier | Equipment fault detection (fault / no fault) |
| Batch Normalisation | Stabilising training on non-stationary grid sensor data |
| Optimizers | Convergence speed for large smart meter datasets |

---

## Background

**Ankit Gupta** — AI/ML Engineer with power domain expertise   
7+ years · Power Distribution(O&M) · JVVNL, Rajasthan Energy Department  
Currently building expertise in deep learning applied to power systems and smart grid analytics.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://linkedin.com/in/ankkit666)
[![Kaggle](https://img.shields.io/badge/Kaggle-Notebooks-blue)](https://kaggle.com/annkitgupta)

---

*This repository is actively updated as new topics are completed.*
