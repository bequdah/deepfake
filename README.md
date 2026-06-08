# Deepfake Detection - Graduation Project 1

## Project Overview

This repository contains the work for Graduation Project 1, which serves as the foundation for a Multi-Stage Deepfake Detection system with Dual Explainability (GP2).

## Exploratory Data Analysis (EDA)

A full EDA was performed on the dataset to understand the distribution, quality, and characteristics of the images before training.

- Visualized class distributions across Real, GAN, and Diffusion Model images
- Analyzed image properties (size, color channels, pixel statistics)
- Explored sample images from each class

📓 Notebook: `EDA/EDA.ipynb`

## Dataset

- **Total Images:** 52,000
- **Classes:** Real, GAN, Diffusion Model (DM)
- **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/vaqudah/deepfake)

## Baseline Model (ResNet-50)

A binary classification baseline (Real vs Fake) trained on 10,000 images.

| | Details |
|---|---|
| **Model** | ResNet-50 (Pretrained on ImageNet) |
| **Task** | Binary Classification (Real vs Fake) |
| **Train Set** | 8,000 images (4,000 Real + 4,000 Fake) |
| **Test Set** | 2,000 images (1,000 Real + 1,000 Fake) |
| **Epochs** | 10 |
| **Optimizer** | Adam (lr=0.0001) |
| **Best Accuracy** | 99.75% |
| **Final Accuracy** | 99.60% |

## Results

![Loss & Accuracy Curves](baseline/results/baseline_curves.png)

![Confusion Matrix](baseline/results/confusion_matrix.png)

## Repository Structure

```
deepfake/
├── EDA/
│   └── EDA.ipynb
└── baseline/
    ├── resnet50_baseline.ipynb
    ├── results/
    │   ├── baseline_curves.png
    │   └── confusion_matrix.png
    └── model/
        └── resnet50_baseline.pth  (not tracked - too large)
```

## GP2 - Coming Soon

Multi-Stage Deepfake Detection with Dual Explainability including:

- Stage 1: Real vs Fake classification
- Stage 2: GAN vs Diffusion Model classification
- GradCAM Explainability
- FFT Frequency Analysis

## Team Members

| Name |
|---|
| Mohammad AlQudah |
| Saba'a AlAzzam |
| Yazan Zydanyen |
| Hussein Freihat |
