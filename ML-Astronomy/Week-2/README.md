# Week 2 — Baselines & Fully-Connected Networks

> 🚧 **Content coming soon.** This week's concept markdowns and notebooks are being written. The outline below is final and shows exactly what you'll learn.

This week we go from "data is loaded" to "a model makes predictions". First we set a **traditional machine-learning baseline** with scikit-learn — a number every fancier model must beat — then we write our **first neural network** in PyTorch: a fully-connected (dense) network built from `nn.Module`.

---

## Planned Scope

### Part 1 — A Baseline with Scikit-Learn

**Machine learning**
- Converting PyTorch tensors back into NumPy arrays for traditional ML.
- **Image flattening:** reshaping a `(3, 64, 64)` image into a single 1D vector.
- Training a simple classifier (K-Nearest Neighbours or Logistic Regression).
- Evaluating accuracy on the test set; why a baseline matters.

**Astronomy**
- **Surface brightness `I(r)`:** how light is distributed across a galaxy from its centre outward.
- **Isophotes:** contours of constant light intensity. Smooth concentric ellipses for ellipticals; jagged, irregular profiles for spirals (dust lanes, arms).

### Part 2 — Fully-Connected Networks (`nn.Module`)

**Machine learning**
- Creating a model class by inheriting from `nn.Module`.
- The `__init__` method (defining layers) and the `forward` method (how data flows).
- `nn.Linear`: building a simple Multi-Layer Perceptron (dense network).
- Loss functions (`nn.CrossEntropyLoss`) and optimisers (`torch.optim.Adam`).

**Astronomy**
- **Stellar demographics:** why ellipticals look uniform and "red and dead" (old, low-mass stars, little gas) versus why spirals look blue (gas-rich, actively star-forming).
- **The Sérsic profile:** `I(r) ∝ exp(-r^(1/n))`, where the index `n` tells us whether a galaxy is disk-dominated (`n ≈ 1`) or bulge-dominated (`n ≈ 4`).

---

## Planned Project Task

1. Flatten the galaxy images, train a simple scikit-learn classifier, and record the **baseline accuracy**. Discuss why it struggles with complex spatial patterns.
2. Build a 2-layer fully-connected network in PyTorch, pass a single batch through it to verify the setup, and print the model architecture.

---

## Prerequisites

Finish [Week 1](../Week-1/) first — this week assumes you have a working `DataLoader` of galaxy images and are comfortable with tensors, shapes, and devices.

---

⬅️ Back to [track overview](../README.md)
