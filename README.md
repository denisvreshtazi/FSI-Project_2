# 🧠 FSI-Project_2 — Neural Networks

> Second practical assignment for the *Fundamentos de Sistemas Inteligentes (FSI)* course — exploring **neural networks** as the second AI paradigm after the adversarial search work in [Connect_4](https://github.com/denisvreshtazi/Connect_4).

[![Python](https://img.shields.io/badge/python-3-blue)]()
[![ML](https://img.shields.io/badge/topic-Neural%20Networks-red)]()
[![Course](https://img.shields.io/badge/course-FSI%20%23%202-green)]()

---

## 📌 Overview

**Trabajo 2 — Redes neuronales** is the second assignment of the *Fundamentos de Sistemas Inteligentes (FSI)* course at **Universidad de Las Palmas de Gran Canaria**.

Where the first project ([Connect_4](https://github.com/denisvreshtazi/Connect_4)) covered **adversarial search**, this one moves from **symbolic AI** to **connectionist AI**: training a neural network to learn a classification or function-approximation task end-to-end.

## 🎯 Objectives

- Understand the **forward pass** through a multi-layer perceptron
- Implement and tune **backpropagation** with gradient descent
- Experiment with different **network architectures** (depth, width, activations)
- Evaluate the model on **train / validation / test** splits
- Reflect on **overfitting**, **underfitting**, and **early stopping**

## 🗂️ Project Structure

```
FSI-Project_2/
├── *.py            # Network implementation + training loop
├── data/           # Dataset (typically split into train/val/test)
└── results/        # Logs, plots, accuracy curves
```

> ⚠️ The exact file names depend on the original starter code; this is the typical layout for FSI assignments.

## 🚀 Setup & Run

### Prerequisites
- Python 3
- `numpy`
- `matplotlib` (for training-curve plots)
- Optional: `tensorflow` or `pytorch` if the assignment used a framework

```bash
pip install numpy matplotlib
# or, if framework-based:
pip install tensorflow
```

### Run

```bash
python main.py
```

(Adjust the entry-point name to match the actual starter file in this repo.)

## 🧠 Concepts Covered

| Concept | Where it appears |
|---|---|
| **Forward propagation** | `forward()` / `predict()` methods of the network |
| **Activation functions** | sigmoid, tanh, ReLU on hidden layers; softmax on output |
| **Loss functions** | MSE for regression, cross-entropy for classification |
| **Backpropagation** | Manual chain-rule gradient computation |
| **Gradient descent** | Vanilla / mini-batch / SGD with momentum |
| **Hyperparameter tuning** | Learning rate, hidden-layer size, epochs |
| **Train/val/test split** | Generalization vs memorization |

## 📊 Typical Experiments

1. **Single hidden layer** — sweep neuron count, plot train/val accuracy
2. **Multiple hidden layers** — compare depth vs width
3. **Activation function comparison** — sigmoid vs ReLU on the same task
4. **Learning-rate study** — observe divergence at high LR, slow learning at low LR
5. **Overfitting demo** — increase epochs until validation loss diverges from training loss

## 💡 Possible Extensions

- Add **L2 regularization** / **dropout**
- Implement **Adam** optimizer instead of vanilla SGD
- Compare custom NumPy implementation against a **PyTorch / TensorFlow** version on the same dataset
- Apply the same network to a **richer real-world dataset** (Fashion-MNIST, CIFAR-10)

## 🔗 Companion Project

➡️ First FSI assignment (adversarial search): [Connect_4](https://github.com/denisvreshtazi/Connect_4)

## 👤 Author

**Denis Vreshtazi** — [GitHub](https://github.com/denisvreshtazi)
