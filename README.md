# 🧠 Autoencoders & VAEs: Theory + Practice

Welcome! This repository helps you consolidate your **theoretical understanding** of Autoencoders (AEs) and **Variational Autoencoders (VAEs)** with hands-on code, visual illustrations, and links to high-quality GitHub repositories.

---

## 🔧 GitHub Repositories to Practice 

### 1. [AntixK/PyTorch-VAE](https://github.com/AntixK/PyTorch-VAE)
- Comprehensive VAE collection in PyTorch.
- Implements multiple VAE variants (Beta-VAE, Conditional-VAE, etc.).
- Dataset: CelebA.

### 2. [Jackson-Kang/Pytorch-VAE-tutorial](https://github.com/Jackson-Kang/Pytorch-VAE-tutorial)
- Beginner-friendly.
- Jupyter Notebooks with comments.
- Works on MNIST and CIFAR-10.

### 3. [ethanluoyc/pytorch-vae](https://github.com/ethanluoyc/pytorch-vae)
- Minimalist VAE implementation.
- Ideal for dissecting the basics.

---

## 🧠 What Are Autoencoders (AEs)?

Autoencoders are unsupervised neural networks that learn to compress data into a **latent representation** and then reconstruct it.

- **Encoder**: Compresses input.
- **Decoder**: Reconstructs original input.
- **Loss**: Mean squared error (MSE) between input and reconstruction.

### AE Architecture:
![Autoencoder](AE.avif)

*Figure: Encoder compresses input, decoder reconstructs it.*

---

## 🤯 What Are Variational Autoencoders (VAEs)? 

VAEs extend AEs by learning a **distribution** over the latent space instead of a fixed vector.

- Encoder learns \( \mu \) and \( \sigma \) (mean and variance).
- Samples latent vectors from \( \mathcal{N}(\mu, \sigma) \).
- Trains with **reconstruction loss** + **KL divergence**.

### Benefits:
- Generate new data samples.
- Smooth latent space.

### VAE Architecture:
![Variational Autoencoder](VAE.jpg) 

*Figure: VAE introduces stochastic sampling from a latent distribution.*

---

## 📁 Projects
 
### 📌 Project 1: Deep Autoencoder for Fashion MNIST (PyTorch)

**Overview**:
Developed a deep learning autoencoder using PyTorch to reconstruct images from the Fashion MNIST dataset. Demonstrates foundational understanding of unsupervised learning.

**Key Contributions**:
- Built a fully connected deep autoencoder with two-layer encoder and decoder.
- Applied MSE loss function; optimized using Adam.
- Trained for 10 epochs, final validation loss: **0.000207**.
- Visualized input vs reconstructed images with `matplotlib` & `torchvision.utils`.
- Efficient preprocessing & transformation of Fashion MNIST dataset.

**Technical Stack**:
- Frameworks: PyTorch, Torchvision
- Techniques: Autoencoders, Image Reconstruction
- Tools: tqdm, DataLoader, GPU acceleration

**Outcome**:
Achieved high-fidelity image reconstruction and deepened practical knowledge of latent space representations and training neural nets.

---

### 📌 Project 2: Variational Autoencoder (VAE) on MNIST

**Overview**:
Built a VAE from scratch using PyTorch to learn a compressed latent representation of MNIST digits. Focused on both image reconstruction and new sample generation.

**Key Features**:
- Custom architecture with 2D latent space (input: 784-dim).
- Decoder: non-linear layers + Sigmoid output.
- Reparameterization trick for stochastic sampling.

**Loss Function**:
- Binary Cross-Entropy (reconstruction) + KL Divergence (regularization).

**Training**:
- 50 epochs, Adam optimizer (lr = 0.001).
- Smooth convergence and strong reconstructions.

**Visualizations**:
- Input image grid and reconstructed comparisons.
- Digit generation from latent vectors.
- Latent space manifold exploration.

**Outcome**:
- Realistic digit generation.
- Strong unsupervised learning performance.
- Gained experience in PyTorch and deep generative models.

**Skills Highlighted**:
- PyTorch · Latent Space Modeling · Autoencoder Design
- Variational Inference · Visualization · Model Optimization

---

## 📚 Summary Table

| Feature             | Autoencoder (AE)         | Variational Autoencoder (VAE)        |
|---------------------|--------------------------|---------------------------------------|
| Latent Space        | Fixed Vector             | Distribution (\( \mu, \sigma \))     |
| Generative?         | ❌                       | ✅                                     |
| Loss Function       | MSE                      | BCE + KL Divergence                   |

---

## 📂 How to Use This Repo

1. Clone any of the above repos or use project folders.
2. Train on Fashion MNIST or MNIST.
3. Visualize reconstructions & latent vectors.
4. Modify encoder/decoder for deeper learning.

---

🎓 Happy Learning!
