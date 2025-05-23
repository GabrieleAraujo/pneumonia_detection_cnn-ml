[![GitHub issues](https://img.shields.io/github/issues/GabrieleAraujo/pneumonia-detection)](https://github.com/GabrieleAraujo/pneumonia_detection/issues)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-blue.svg?style=flat-square)](https://github.com/GabrieleAraujo/pneumonia-detection/pulls)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![HitCount](https://views.whatilearened.today/views/github/GabrieleAraujo/pneumonia-detection.svg)](https://github.com/GabrieleAraujo/pneumonia-detection) 
[![website coderjojo.github.io](https://img.shields.io/website-up-down-yellow-red/http/coderjojo.github.io/creative-profile-readme.svg)](http://laca-ufopa.com.br/)

<h1 align="center">
  <img align="center" alt="FedCSIS" height="200" width="2200" src="https://2025.fedcsis.org/sites/2025/files/Fedcsis2025-2400x300.png"> <br>

  <br>
   Hybrid Approaches for Pneumonia Detection in X-rays: Combining CNNs and ML Classifiers
  <br>
</h1>

<h4 align=“center”>This repository contains the databases and results of the article submitted to the 20th Conference on Computer Science and Intelligence Systems FedCSIS 2025 (IEEE#66292) (<a href=“[https://www.sbcas2025.com/](https://2025.fedcsis.org/)”>FedCSIS 2025</a>)</h4>

<p align="center">
  <a href="#abstract">Abstract</a> •
  <!-- <a href="#overview">Overview</a> •
  <a href="#conteúdo">Conteúdo</a> • -->
  <!-- <a href="#autores">Autores</a> -->
</p>

## Abstract

Pneumonia is a disease that impacts millions of people worldwide, and X-ray image detection is one of the primary diagnostic tools used. This study presents a hybrid diagnostic approach combining Convolutional Neural Networks (CNNs) with traditional classifiers, namely Random Forest (RF) and Support Vector Machine (SVM), to detect pneumonia from chest X-ray images. Features were extracted from MobileNetV2, VGG16, and EfficientNetB0 and used to train RF and SVM models with hyperparameter tuning via GridSearchCV. Ensemble models were also explored: (i) CNNs + RF, (ii) CNNs + SVM, and (iii) RF + SVM. Experiments were conducted using a public pediatric dataset (5.856 X-rays) with stratified k-fold cross-validation and data augmentation. CNNs + RF achieved the highest 0.977 AUC and 91.9\% accuracy, while individual models, VGG16, showed competitive performance (91.8\% accuracy, 0.969 AUC). Results were statistically validated and showed strong potential for clinical support, particularly in settings with limited resources. In future work, we propose extending the approach to multiclass classification and refining model optimization strategies.

---

OBS.: **The remaining sections of this repository will be made available after the article's official publication.**


<!--
Key findings:
- **CNNs + RF** achieved the best performance: **91.9% accuracy, AUC = 0.977**;
- **CNNs + SVM** achieved the best recall: **0.979**, reducing false negatives;
- Statistical tests confirmed the significance of the results.

The results suggest this hybrid pipeline is suitable for deployment in **low-resource clinical environments**.  
Future work includes multiclass classification and improved ensemble strategies.
-->
---

## Repository Structure
```bash 
pneumonia-detection/
├── data/ # Input dataset and preprocessed versions
├── figures/ # Confusion matrices and performance plots
├── notebooks/ # Jupyter notebooks for training & evaluation
├── models/ # Saved model weights (optional)
├── results/ # Output metrics, AUC scores, logs, etc.
├── utils/ # Helper scripts: preprocessing, metrics, etc.
├── requirements.txt # Python dependencies
└── README.md
```
---
<!--
## Dataset

We used the [Chest X-ray dataset by Kermany et al. (2018)](https://data.mendeley.com/datasets/rscbjbr9sj/3), containing:
- 5.856 pediatric chest X-rays (normal and pneumonia)
- Data balanced and preprocessed
- Augmented using rotations, flips, shifts, and brightness changes
-->
## Pipeline


## Results Summary
<!--
### Best performing models

| Model         | Accuracy | Recall | F1-score | AUC   |
|---------------|----------|--------|----------|--------|
| CNNs + RF     | **91.9%** | 91.9%  | 91.8%    | **0.977** |
| CNNs + SVM    | 89.7%    | **97.9%** | 91.7%    | 0.963 |
| VGG16         | 91.8%    | 91.8%  | 91.7%    | 0.969 |
-->
---

## How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/GabrieleAraujo/pneumonia-detection.git
   cd pneumonia-detection

2. Create a virtual environment and install dependencies:
   ```bash
   pip install -r requirements.txt
4. Run the notebooks inside `/notebooks/` for training and evaluation:

## License
This project is licensed under the MIT License.


