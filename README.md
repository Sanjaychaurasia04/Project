# CIFAR-10 Image Classification Challenge

## 🎯 Overview
This repository contains a **CIFAR-10 image classification project** developed **entirely on Google Colab**.  
Each level is implemented as a **public Colab notebook**, allowing **one-click execution with visible outputs**.

The project demonstrates progressive learning across:
- Transfer Learning
- Improved CNN training
- Custom Attention-based architectures
- Ensemble Learning (Level 4)

---

## 📊 Results Summary

| Level | Model / Technique | Target Accuracy | Achieved Accuracy | Epochs |
|------|------------------|-----------------|------------------|--------|
| Level 1 | ResNet18 (Transfer Learning) | ≥85% | **89.31%** | 5 |
| Level 2 | ResNet34 (Improved Training) | ≥90% | 87.47% | 5 |
| Level 3 | Custom CNN + Attention | ≥91% | 84.11% | 12 |
| Level 4 | Ensemble Learning | ≥93% | Scalable* | 10 / model |

\* *Accuracy improves with higher epochs (30–50 per model).*

---

## 🎮 Google Colab Notebooks (One-Click Run)

All experiments were executed on **Google Colab**.  
Notebooks are **public**, **fully executable**, and **outputs are visible**.

| Level | Open in Colab | Runtime |
|------|---------------|---------|
| Level 1 | [Open Notebook](https://colab.research.google.com/drive/14H9qdOhpK8kbmTQbz7SVNkjioGRTm-0V) | CPU |
| Level 2 | [Open Notebook](https://colab.research.google.com/drive/1XO3Fg3eX5ukG-V-r2PqbGHblQj3TkFO_) | GPU (T4) |
| Level 3 | [Open Notebook](https://colab.research.google.com/drive/1dzyGdEliG7s50xz2pVDElWN_kcpvEFBA) | GPU (T4) |
| Level 4 | [Open NodeBook](https://colab.research.google.com/drive/1jHe3bZsCA-8kS8gbhzXToS6Px2ShQaSA?usp=sharing) | GPU (Colab) |

---

## 🏗️ Repository Structure

Project
├── terafac.ipynb
│── Level2.ipynb
│── Level3.ipynb
│── Level4.ipynb


---

## 🧠 Level-wise Approach

### Level 1 – Transfer Learning
- ResNet18 pre-trained on ImageNet
- Modified for CIFAR-10
- Fast convergence with limited epochs

### Level 2 – Improved Training
- ResNet34 backbone
- Strong data augmentation
- AdamW optimizer + Cosine Annealing

### Level 3 – Custom Attention CNN
- Lightweight CNN built from scratch
- Channel & Spatial Attention
- Parameter-efficient (~1.79M params)

### Level 4 – Ensemble Learning
- Combines predictions from multiple models
- Reduces individual model errors
- Improves generalization


---

## 📚 Dataset
**CIFAR-10**
- 60,000 RGB images (32×32)
- 10 balanced classes
- Loaded using torchvision

---

## 🧪 Reproducibility
All notebooks use fixed seeds and consistent splits.

```python
torch.manual_seed(42)
numpy.random.seed(42)

```



