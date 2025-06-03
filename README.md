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

## 📚 Summary
| Feature             | Autoencoder (AE)         | Variational Autoencoder (VAE)        |
|---------------------|--------------------------|---------------------------------------|
| Latent Space        | Fixed Vector             | Distribution (\( \mu, \sigma \))     |
| Generative?         | ❌                       | ✅                                     |
| Loss Function       | MSE                      | MSE + KL Divergence                   |

---

## 📂 How to Use This Repo

1. Clone any of the above repos.
2. Run on MNIST or your dataset.
3. Observe reconstructions & generated samples.
4. Try modifying the encoder/decoder depth.

Happy Learning! 🎓
