# Quantum Neural Network for Image Classification

A hybrid quantum-classical neural network for handwritten digit classification using the **MNIST dataset**, built with **Python, PyTorch, and PennyLane**.

## Overview

This project demonstrates how **Quantum Neural Networks (QNNs)** can be integrated with classical deep learning for image classification.

The model follows a hybrid architecture:

```text
MNIST Image (28×28)
        ↓
Resize to 4×4
        ↓
16 Pixel Features
        ↓
Classical Neural Network
16 → 8 → 4
        ↓
Angle Encoding
        ↓
4-Qubit Quantum Circuit
        ↓
RY + RZ + CNOT Gates
        ↓
Quantum Measurements
        ↓
Classical Classifier
4 → 10
        ↓
Digit Prediction (0–9)
```
## Key Components

- **Dataset:** MNIST handwritten digits
- **Image size:** 28×28 → 4×4
- **Qubits:** 4
- **Quantum circuit:** Variational Quantum Circuit
- **Encoding:** Angle encoding using `RY` gates
- **Quantum gates:** `RY`, `RZ`, and `CNOT`
- **Entanglement:** CNOT gates
- **Measurement:** Pauli-Z expectation values
- **Classical framework:** PyTorch
- **Quantum framework:** PennyLane
- **Optimizer:** Adam
- **Loss:** Cross Entropy Loss
- **Classes:** 10 digits (0–9)

## Results

The model was trained on **5,000 MNIST images** and evaluated on **1,000 test images**.

**Test Accuracy: 36.90%**

The project also includes:

- Training loss graph
- Training accuracy graph
- Quantum circuit visualization
- Confusion matrix
- Sample predictions

## Why Hybrid Quantum-Classical?

The classical neural network performs feature reduction, while the quantum circuit processes the reduced features using parameterized quantum gates and entanglement.

This hybrid approach allows quantum computing concepts to be incorporated into a practical machine learning workflow.

## Technologies

- Python
- PyTorch
- PennyLane
- Torchvision
- NumPy
- Matplotlib
- Scikit-learn

## Project File

```text
Quantum_Neural_Network_Image_Classification/
│
├── Quantum_Neural_Networks_for_Image_Classification.ipynb
└── README.md
```

