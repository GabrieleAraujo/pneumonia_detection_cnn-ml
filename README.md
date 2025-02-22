# pneumonia_detection

<h1 align="center">
  <img align="center" alt="SBSI" height="80" width="280" src="https://sbsi2024.ufjf.br/assets/images/sbsi2024.png"> <br>
  <br>
   Hybrid Approaches for Pneumonia Detection in X-rays: Combining CNNs and Random Forest
  <br>
</h1>

<h4 align="center">Este repositório contém as bases de dados e resultados do artigo submetido ao <br> XXV Simpósio Brasileiro de Computação Aplicada à Saúde (<a href="https://jems3.sbc.org.br/sbcas2025">SBCAS 2025</a>)</h4>

<p align="center">
  <a href="#abstract">Abstract</a> •
  <!-- <a href="#overview">Overview</a> •
  <a href="#conteúdo">Conteúdo</a> • -->
  <!-- <a href="#autores">Autores</a> -->
</p>

## Abstract

Pneumonia is a disease that impacts millions of people worldwide, and X-ray image detection is one of the primary diagnostic tools used. This study proposes an approach based on Ensemble Learning that combines Convolutional Neural Networks (CNNs) with Random Forest (RF) for the automated classification of chest X-ray images. A dataset containing 5.856 images was utilized to implement and compare various architectures, including MobileNetV2, EfficientNetB0, and VGG16. The results indicate that EfficientNetB0 underperformed, while the Ensemble (All) model achieved the highest AUC (0.9705), and RF obtained the best accuracy (90.71%). Statistical tests confirmed significant differences between models. These findings reinforce the effectiveness of hybrid approaches in medical image classification.