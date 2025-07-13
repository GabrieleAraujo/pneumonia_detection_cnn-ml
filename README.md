[![GitHub issues](https://img.shields.io/github/issues/GabrieleAraujo/pneumonia_detection_cnn-ml)](https://github.com/GabrieleAraujo/pneumonia_detection_cnn-ml/issues)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-blue.svg?style=flat-square)](https://github.com/GabrieleAraujo/pneumonia_detection_cnn-ml/pulls)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![HitCount](https://views.whatilearened.today/views/github/GabrieleAraujo/pneumonia_detection_cnn-ml.svg)](https://github.com/GabrieleAraujo/pneumonia_detection_cnn-ml) 
[![website coderjojo.github.io](https://img.shields.io/website-up-down-yellow-red/http/coderjojo.github.io/creative-profile-readme.svg)](http://laca-ufopa.com.br/)

<h1 align="center">
  <img align="center" alt="FedCSIS" height="180" width="2200" src="https://2025.fedcsis.org/sites/2025/files/Fedcsis2025-2400x300.png"> <br>

  <br>
   Hybrid Approaches for Pneumonia Detection in X-rays: Combining CNNs and ML Classifiers
  <br>
</h1>

<h4 align=“center”>This repository contains the databases and results of the article submitted to the 20th Conference on Computer Science and Intelligence Systems FedCSIS 2025 (IEEE#66292) (<a href="https://www.sbcas2025.com/](https://2025.fedcsis.org/">FedCSIS 2025</a>)</h4>

<p align="center">
  <a href="#abstract">Abstract</a> •
  <a href="#repository">Repository</a> •
  <a href="#pipeline">Pipeline</a> •
  <a href="#dataset">Dataset</a> •
  <a href="#results">Results</a> •
  <a href="#authors">Authors</a> 
</p>

## Abstract

Pneumonia is a disease that impacts millions of people worldwide, and X-ray image detection is one of the primary diagnostic tools used. This study presents a hybrid diagnostic approach combining Convolutional Neural Networks (CNNs) with traditional classifiers, namely Random Forest (RF) and Support Vector Machine (SVM), to detect pneumonia from chest X-ray images. Features were extracted from MobileNetV2, VGG16, and EfficientNetB0 and used to train RF and SVM models with hyperparameter tuning via GridSearchCV. Ensemble models were also explored: (i) CNNs + RF, (ii) CNNs + SVM, and (iii) RF + SVM. Experiments were conducted using a public pediatric dataset (5.856 X-rays) with stratified k-fold cross-validation and data augmentation. CNNs + RF achieved the highest 0.977 AUC and 91.9\% accuracy, while individual models, VGG16, showed competitive performance (91.8\% accuracy, 0.969 AUC). Results were statistically validated and showed strong potential for clinical support, particularly in settings with limited resources. In future work, we propose extending the approach to multiclass classification and refining model optimization strategies.


---

## Repository
```bash 
pneumonia-detection/
├── results/  
└── README.md
```
## Pipeline
The following diagram summarizes the pipeline used in this study:

<p align="center">
  <img src="https://github.com/GabrieleAraujo/pneumonia_detection_cnn-ml/blob/main/Pipeline.png" alt="Pipeline Diagram" width="800"/>
</p>

---

## Dataset
- [Chest Xray-pneumonia](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia) 

---

## Results

### Performance metrics for individual and ensemble models (Proposed and Literature)

| Model                                          | Accuracy | Precision | Recall (Sens.) | F1-score | F1-macro | AUC   |
|-----------------------------------------------|----------|-----------|----------------|----------|----------|-------|
| **Literature Models**                         |          |           |                |          |          |       |
| Tougaccar et al. (2020) – VGG16 + SVM          | 0.967    | 0.966     | 0.968          | 0.967    | --       | --    |
| Akgundogdu et al. (2021) – 2D DWT + RF         | 0.971    | 0.990     | 0.917          | 0.980    | 0.926    | 0.990 |
| Akgundogdu et al. (2021) – 2D DWT + SVM        | 0.934    | 0.946     | 0.852          | 0.875    | 0.830    | 0.908 |
| El Asnaoui et al. – Hybrid (EffNetB0 + SVM)    | 0.970    | 1.000     | 0.958          | 0.979    | --       | 0.980 |
| El Asnaoui et al. – EfficientNetB0 (sigmoid)   | 0.967    | 0.999     | 0.956          | 0.977    | --       | 0.976 |
| Kermany et al. (2018) – InceptionV3 + TL       | 0.928    | 0.901     | 0.932          | 0.928    | --       | 0.968 |
| **Proposed Models**                           |          |           |                |          |          |       |
| MobileNetV2                                    | 0.889    | 0.893     | 0.889          | 0.887    | 0.877    | 0.954 |
| VGG16                                          | 0.918    | 0.921     | 0.918          | 0.917    | 0.911    | 0.969 |
| EfficientNetB0                                 | 0.896    | 0.898     | 0.896          | 0.896    | 0.890    | 0.963 |
| Random Forest                                  | 0.878    | 0.882     | 0.878          | 0.875    | 0.864    | 0.945 |
| Ensemble CNNs + RF                             | 0.919    | 0.921     | 0.919          | 0.918    | 0.911    | 0.977 |
| Ensemble MN + VGG + RF                         | 0.911    | 0.915     | 0.911          | 0.909    | 0.901    | 0.974 |
| Ensemble CNNs + SVM                            | 0.897    | 0.862     | 0.979          | 0.917    | 0.889    | 0.963 |
| Ensemble RF + SVM                              | 0.724    | 0.725     | 0.724          | 0.703    | 0.670    | 0.802 |



<!--
### Best performing models
-->
---
## How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/GabrieleAraujo/pneumonia_detection_cnn-ml.git
   cd pneumonia-detection

2. Create a virtual environment and install dependencies:
   ```bash
   pip install -r requirements.txt
4. Run the notebooks inside `/notebooks/` for training and evaluation:

## License
This project is licensed under the MIT License.

## Authors

<table>
  <tr>
    <td align="center">
      <a href="https://orcid.org/0000-0003-1143-507X">
        <img src="https://media.licdn.com/dms/image/v2/D4D03AQGjSwuxOtcWTA/profile-displayphoto-shrink_200_200/B4DZTYABOEGcAc-/0/1738790672659?e=1753315200&v=beta&t=w9ElVgj2tNOaCe4zkQ04e8WxDn42IXRvOZ-ZFYm0H5g" width="100px;" alt="Foto da Gabriele"/><br>
        <sub>
          <b>Gabriele S. Araújo</b><br>
          UEMA – São Luís, Brazil
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://orcid.org/0000-0002-5805-2490">
        <img src="https://media.licdn.com/dms/image/v2/C5603AQHhhmqwVwA1Dw/profile-displayphoto-shrink_200_200/profile-displayphoto-shrink_200_200/0/1516527015507?e=1753315200&v=beta&t=xyq4UPwcLyiYUcrSs6AvX2obdZd4Tfo3jlxIuWp5FFM" width="100px;" alt="Foto do Omar"/><br>
        <sub>
          <b>Omar Andres C. Cortes</b><br>
          IFMA – São Luís, Brazil
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://orcid.org/0000-0003-1977-1641">
        <img src="https://media.licdn.com/dms/image/v2/C5603AQF-p0kzl_K75w/profile-displayphoto-shrink_200_200/profile-displayphoto-shrink_200_200/0/1517004464388?e=1753315200&v=beta&t=sevBH_b4ISWysiW_91E7FL8AOzWfE19DNtsUJvxl5ZA" width="100px;" alt="Foto do Olaf"/><br>
        <sub>
          <b>Olaf Reinhold</b><br>
          DHSN Riesa – Germany
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://orcid.org/0000-0002-6282-0368">
        <img src="https://avatars.githubusercontent.com/u/42838538?s=400&v=4" width="100px;" alt="Foto do Fábio"/><br>
        <sub>
          <b>Fábio M. F. Lobato</b><br>
          UFOPA – Santarém, Brazil
        </sub>
      </a>
    </td>
  </tr>
</table>

