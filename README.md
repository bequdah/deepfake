\# Deepfake Detection - Graduation Project 1



\## Project Overview

This repository contains the work for Graduation Project 1, which serves as the foundation for a Multi-Stage Deepfake Detection system with Dual Explainability (GP2).



\## Dataset

\- \*\*Total Images:\*\* 52,000

\- \*\*Classes:\*\* Real, GAN, Diffusion Model (DM)

\- \*\*Source:\*\* \[Kaggle Dataset](https://www.kaggle.com/datasets/vaqudah/deepfake)



\## Baseline Model (ResNet-50)

A binary classification baseline (Real vs Fake) trained on 10,000 images.



| | Details |

|---|---|

| \*\*Model\*\* | ResNet-50 (Pretrained on ImageNet) |

| \*\*Task\*\* | Binary Classification (Real vs Fake) |

| \*\*Train Set\*\* | 8,000 images (4,000 Real + 4,000 Fake) |

| \*\*Test Set\*\* | 2,000 images (1,000 Real + 1,000 Fake) |

| \*\*Epochs\*\* | 10 |

| \*\*Optimizer\*\* | Adam (lr=0.0001) |

| \*\*Best Accuracy\*\* | 99.75% |

| \*\*Final Accuracy\*\* | 99.60% |



\## Results

![Loss & Accuracy Curves](baseline/results/baseline_curves.png)

![Confusion Matrix](baseline/results/confusion_matrix.png)



\## Repository Structure

```

deepfake/

└── baseline/

&#x20;   ├── baseline.ipynb

&#x20;   ├── results/

&#x20;   │   ├── baseline\_curves.png

&#x20;   │   └── confusion\_matrix.png

&#x20;   └── models/

&#x20;       └── resnet50\_baseline.pth

```



\## GP2 - Coming Soon

Multi-Stage Deepfake Detection with Dual Explainability including:

\- Stage 1: Real vs Fake classification

\- Stage 2: GAN vs Diffusion Model classification

\- GradCAM Explainability

\- FFT Frequency Analysis



## Team Members

| Name |
|---|
| Mohammad AlQudah |
| Saba'a AlAzzam |
| Yazan Zydanyen |
| Hussein Freihat |

