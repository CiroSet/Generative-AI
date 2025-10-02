# 🧬 FaceForge – Conditional Generative Models for Human Faces

FaceForge is an exploration of **Generative AI** applied to face synthesis.  
The goal: generate realistic **64×64 face images** from the [CelebA dataset](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html), conditioned on **semantic attributes**:

- 👩‍🦰 Gender (Male / Female)  
- 👓 Eyeglasses (Yes / No)  
- 🧔 Beard (Yes / No)  

I implemented **three different generative paradigms** to compare their strengths:  

- 🌀 **Variational Autoencoder (VAE)**  
- ⚡ **Generative Adversarial Network (GAN)**  
- 🌫️ **Diffusion Model**  

---

## ✨ Highlights

- **Conditional generation**: steer synthesis with attributes (e.g. *“female, glasses, no beard”*).  
- **Three models, one task**: side-by-side comparison of VAE, GAN, and Diffusion.  
- **Lightweight resolution**: 64×64 for fast experiments, extendable to higher res.  
- **Reproducible setup**: clean configs, deterministic seeds, ready-to-run scripts.  

---

## 🖼️ Example Results

| Condition (gender, glasses, beard) | Samples |
|-----------------------------------|---------|
| (0,0,0) Female, No glasses, No beard | ![sample1](out/example1.png) |
| (1,1,1) Male, Glasses, Beard         | ![sample2](out/example2.png) |

*(more results coming soon…)*

---

## ⚙️ Setup

```bash
git clone https://github.com/your-username/faceforge.git
cd faceforge

python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
