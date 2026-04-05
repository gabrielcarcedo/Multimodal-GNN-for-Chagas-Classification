# Multimodal Graph Learning for Chagas Disease Classification

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

This repository contains the official implementation of the paper **"Multimodal Graph Learning for Chagas Disease Classification"**.

We present a comprehensive computational framework that integrates Machine Learning (ML) feature selection, generative data augmentation via Variational Graph Autoencoders (VGAE), and classification using Graph Attention Networks (GAT). This approach is specifically designed to address the challenges of high-dimensional, small-sample biomedical data in classifying the stages of *Trypanosoma cruzi* infection in a multimodal experimental murine model.

## Overview

Chagas disease, caused by the protozoan *T. cruzi*, is a major public health challenge in Latin America. Early and accurate detection of infection stages (Acute vs. Chronic) is critical. This project utilizes a multimodal dataset (ECG, ECHO, Doppler, and ELISA) and proposes a novel pipeline:

1.  **Feature Selection (FS):** Identification of the most discriminative biomarkers using a voting scheme based on traditional ML classifiers.
2.  **Data Augmentation (FS-VGAE):** Generation of synthetic subject data using a Variational Graph Autoencoder to overcome the "Small Data" limitation while preserving biological covariance.
3.  **Classification (GAT):** Utilizing Graph Attention Networks on fully connected graphs to capture nonlinear dynamic interactions between multimodal parameters.
4.  **Interpretability (GNNExplainer):** *Post-hoc* analysis to validate the pathophysiological consistency of the model's decisions, revealing the most relevant clinical features for classification.

Our FS-VGAE + GAT framework achieves state-of-the-art performance, including 100% AUROC in identifying the stage of infection.

## Authors and Affiliations

* **Gabriel Carcedo-Rodríguez**$^{1}$ (gabrielcarcedo@comunidad.unam.mx)
* **Erik Molino-Minero-Re**$^{2}$ (erik.molino@iimas.unam.mx)
* **Jorge Perez-Gonzalez**$^{2}$ (jorge.perez@iimas.unam.mx)
* **Nidiyare Hevia-Montiel**$^{2}$* (nidiyare.hevia@iimas.unam.mx)

$^{1}$ *Master Program in Computer Science and Engineering, Universidad Nacional Autónoma de México, Mérida, Yucatán, México.*
$^{2}$ *Unidad Académica del Instituto de Investigaciones en Matemáticas Aplicadas y en Sistemas, Universidad Nacional Autónoma de México, Mérida, Yucatán, México.*

\* *Corresponding Authors*

**Acknowledgements**
-Gabriel Carcedo-Rodríguez is grateful to SECIHTI for the scholarship received (CVU 2054635).
-Special thanks to PhD. Paulina Haro from the Veterinary Science Research Institute, UABC, for her invaluable clinical advice.
-This work was supported by UNAM-PAPIIT programs: IT101225, IN102626, and IG101725.

*License*
This project is licensed under the MIT License - see the https://www.google.com/search?q=LICENSE file for details.
