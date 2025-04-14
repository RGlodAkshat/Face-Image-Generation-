# 🎨 Fake Image Generation using GANs & VAEs

Welcome to the **Fake Image Factory™** — where neural nets dream up pixels like Picasso on steroids. In this repo, I’ve built two powerful generative models from scratch using **PyTorch**:

> ✅ A classic **GAN (Generative Adversarial Network)**  
> ✅ A mind-bending **VAE (Variational Autoencoder)**

Both trained on the OG **MNIST dataset** to generate fake handwritten digits that look hella real.

---

## 🚀 Projects Included

### 1. GAN - Generative Adversarial Network
- Two players: **Generator** (the faker) vs **Discriminator** (the detective)
- Trained using **Binary Cross Entropy loss**
- Generator learns to create digits from pure noise (aka chaos magic ⚡)
- Discriminator tries to tell real from fake
- Over time, Generator becomes so good it fools the Discriminator!

📂 File: `gan_mnist.py`

### 2. VAE - Variational Autoencoder
- Learns to compress and then reconstruct images (encoding-decoding vibes)
- Trains using **reconstruction loss** + **KL divergence**
- The latent space is **continuous**, so we can generate new digits by sampling from it
- More stable than GANs but less "crispy" results

📂 File: `vae_mnist.py`

---

## 🧠 Concepts Used

- PyTorch (obviously)
- Custom neural networks with `nn.Module`
- Loss functions: BCE, MSE, KL Divergence
- Data loading with `torchvision.datasets.MNIST`
- Latent space sampling for VAE
- DCGAN-style architecture for GAN

---

## 📸 Some Generated Samples

> Add some output images here if possible — like side-by-side real vs fake for flex.

---

## 🛠️ How to Run

```bash
# Clone the repo
git clone https://github.com/yourusername/fake-image-generation
cd fake-image-generation

# Install requirements
pip install torch torchvision matplotlib

# Run GAN
python gan_mnist.py

# Run VAE
python vae_mnist.py
