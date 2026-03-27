# Weight Initialization Comparison with tanh (Glorot vs Random)

## Overview
This project explores how different **weight initialization techniques** affect neural network training when using **tanh activation function**.

Improper initialization can cause issues such as:
- Vanishing gradients
- Slow convergence
- Poor training performance

This experiment compares **Random Initialization** with **Glorot (Xavier) Initialization** to analyze how each method influences training behavior.

All experiments and visualizations are implemented in a Jupyter Notebook.

---

## Objectives

The goals of this project are:

- Understand the importance of weight initialization in neural networks
- Compare **Random Initialization** and **Glorot Initialization**
- Observe their effect on:
  - training convergence
  - gradient flow
  - stability of learning
- Visualize performance differences using plots

---

## Weight Initialization Methods

### Random Initialization
Weights are initialized randomly without considering the number of input and output neurons.

Problems:
- Can lead to **vanishing gradients**
- Training becomes unstable for deeper networks
- Slow learning

---

### Glorot (Xavier) Initialization
Glorot initialization scales the weights based on the number of neurons in the previous and next layers.

Formula:

```
Var(W) = 2 / (n_in + n_out)
```

Benefits:
- Maintains consistent variance of activations across layers
- Reduces vanishing/exploding gradient problems
- Improves convergence speed

---

## Experiment Setup

- Activation Function: **tanh**
- Model: Fully connected neural network
- Initialization methods compared:
  - Random Initialization
  - Glorot Initialization
- Implemented using **Python and NumPy**

---

## Results

The experiment demonstrates that:

- **Random Initialization**
  - slower convergence
  - unstable gradient propagation

- **Glorot Initialization**
  - faster convergence
  - more stable training
  - improved gradient flow

Visualization plots in the notebook show how the two initialization strategies differ during training.

---

## Repository Structure

```
Weight-Initialization-Comparison-with-tanh-using-Glorort/
│
├── Weight Initialisation Comparison.ipynb
└── README.md
```

---

## How to Run

1. Clone the repository

```
git clone https://github.com/kanisk29/Weight-Initialization-Comparison-with-tanh-using-Glorort.git
```

2. Navigate to the folder

```
cd Weight-Initialization-Comparison-with-tanh-using-Glorort
```

3. Open the notebook

```
jupyter notebook
```

4. Run the notebook cells to reproduce the experiment.

---

## Key Takeaways

- Weight initialization plays a critical role in neural network training.
- Poor initialization can lead to **vanishing gradients** and slow learning.
- **Glorot Initialization** significantly improves training stability when using **tanh activation**.

---

## Future Improvements

Possible extensions for this project:

- Compare with **He Initialization**
- Test with different activation functions (ReLU, LeakyReLU)
- Run experiments on deeper neural networks
- Compare training loss curves more extensively

---

## Author

**Kanisk Dasgupta**
