# Quantum Neural Network for MNIST Classification

A Quantum Neural Network (QNN) implemented in Qiskit that classifies handwritten digits from the MNIST dataset. This project introduces a novel **white/black amplitude encoding** scheme that preserves edge pixel information lost by standard normalization.

## Results
- **96% test accuracy** on binary digit classification (0 vs 1)
- Only **24 trainable parameters** vs ~2,625 in a classical equivalent
- Loss decreased monotonically from 1.13 → 0.27 over 15 epochs

## Architecture
- 11-qubit parameterized quantum circuit
- RY rotation gates + real amplitudes ansatz (full entanglement)
- Parameter-shift rule for gradient computation
- Hybrid quantum-classical training loop via Qiskit + PyTorch

## Based On
Co-authored research paper: *A Study of Quantum Neural Networks in Machine Learning* (2026)

## Setup
```bash
pip install qiskit qiskit-aer qiskit-machine-learning torch torchvision numpy matplotlib scikit-learn
```
Open `qnn_mnist.ipynb` in Jupyter or VS Code and run cells sequentially.

##
Research paper - 
