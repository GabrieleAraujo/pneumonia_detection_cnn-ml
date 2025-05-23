

<h1 align="center">
  <br>
   Hybrid Approaches for Pneumonia Detection in X-rays: Combining CNNs and ML Classifiers
  <br>
</h1>

<h4 align=“center”>This repository contains the databases and results of the article submitted to the <br> 20th Conference on Computer Science and Intelligence Systems FedCSIS 2025 (IEEE#66292) (<a href=“[https://www.sbcas2025.com/](https://2025.fedcsis.org/)”>FedCSIS 2025</a>)</h4>

<p align="center">
  <a href="#abstract">Abstract</a> •
  <!-- <a href="#overview">Overview</a> •
  <a href="#conteúdo">Conteúdo</a> • -->
  <!-- <a href="#autores">Autores</a> -->
</p>

## Abstract

Pneumonia is a disease that impacts millions of people worldwide, and X-ray image detection is one of the primary diagnostic tools used. This study presents a hybrid diagnostic approach combining Convolutional Neural Networks (CNNs) with traditional classifiers, namely Random Forest (RF) and Support Vector Machine (SVM), to detect pneumonia from chest X-ray images. Features were extracted from MobileNetV2, VGG16, and EfficientNetB0 and used to train RF and SVM models with hyperparameter tuning via GridSearchCV. Ensemble models were also explored: (i) CNNs + RF, (ii) CNNs + SVM, and (iii) RF + SVM. Experiments were conducted using a public pediatric dataset (5.856 X-rays) with stratified k-fold cross-validation and data augmentation. CNNs + RF achieved the highest 0.977 AUC and 91.9\% accuracy, while individual models, VGG16, showed competitive performance (91.8\% accuracy, 0.969 AUC). Results were statistically validated and showed strong potential for clinical support, particularly in settings with limited resources. In future work, we propose extending the approach to multiclass classification and refining model optimization strategies.
