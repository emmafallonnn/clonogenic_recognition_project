# Automated Clonogenic Assay Analysis

This repository accompanies the publication:

**Quantifying Measurement Bias in Clonogenic Survival Assays Using Automated Colony Detection and Synthetic Benchmarking**

## Overview

This project implements an automated image-analysis pipeline for clonogenic assays using classical computer vision techniques. The workflow performs colony segmentation, quantitative evaluation, and benchmarking on both synthetic and experimental datasets.

The repository provides code to:

- Generate synthetic clonogenic assay datasets with ground-truth masks
- Perform automated colony segmentation
- Evaluate segmentation performance using Dice, IoU, Precision and Recall
- Produce publication-quality figures
- Analyse experimental clonogenic assay images
- Compare predictions against manually annotated masks
- Compute ROC curves and AUC values

---

## Repository Structure

```
codeforpublication.ipynb      Main analysis notebook
data/                         Input datasets
outputs/                      Generated masks, figures and metrics
figures/                      Publication figures
```

---

## Requirements

Python 3.11 (or later)

Main packages:

```
numpy
opencv-python
matplotlib
scikit-image
scikit-learn
scipy
pandas
Pillow
tqdm
```

Install dependencies using

```bash
pip install -r requirements.txt
```

---

## Workflow

The notebook is organised into the following sections:

1. User settings
2. Synthetic dataset generation
3. Synthetic image visualisation
4. Optional image resizing
5. Automated synthetic segmentation
6. Overlay figure generation
7. Synthetic mask comparisons
8. Quantitative segmentation metrics
9. Error-map generation
10. Experimental image segmentation
11. Comparison with manual annotations
12. Experimental Dice and IoU analysis
13. ROC/AUC analysis
14. Experimental error-map visualisation

Each section can be executed independently once the required input data are available.

---

## Input Data

The pipeline expects:

- Synthetic images
- Synthetic ground-truth masks
- Experimental clonogenic assay images
- Manual annotation masks for experimental images

Directory locations can be configured in the **User Settings** section.

---

## Outputs

The pipeline generates:

- Binary segmentation masks
- Overlay visualisations
- Error maps
- Dice, IoU, Precision and Recall metrics
- ROC curves
- Publication-quality figures

---

## Citation

If you use this code in your research, please cite:

> Fallon E., *et al.* Quantifying Measurement Bias in Clonogenic Survival Assays Using Automated Colony Detection and Synthetic Benchmarking. *(Journal information to be added after publication.)*

---
