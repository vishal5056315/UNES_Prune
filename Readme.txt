# UNES-Prune: Brain Tumor Segmentation and Classification

This repository contains the complete implementation of "UNES-Prune", an integrated deep-learning framework for brain tumor segmentation, feature representation, classification, and structured model optimization from MRI images.

## Methodology

The proposed framework consists of three major stages:

1. Tumor Segmentation – U-Net++ is used to generate tumor-region masks.
2. Feature Representation – EfficientNetV2 is used to extract compact 1,536-dimensional feature representations.
3. Tumor Classification – A Swin Transformer is used for hierarchical tumor classification, followed by structured pruning of the MLP intermediate dimension to reduce computational complexity.



Datasets

Two MRI datasets are used:

- Brain Tumour Classification Dataset (Main Dataset) – used for feature extraction and tumor classification.
- LGG MRI Segmentation Dataset – used for supervised U-Net++ tumor segmentation.

The classification experiments use a balanced cohort of **9,600 MRI images** consisting of:

- Glioma: 2,400
- Meningioma: 2,400
- Pituitary: 2,400
- No Tumor: 2,400

The cohort is divided into 8,000 training, 800 validation, and 800 independent test images.

-main_notebook.ipynb – Complete implementation of the UNES-Prune methodology, including model training, pruning, evaluation, and result visualization.

"If you use this code, then please cite this article: [ Optimizing Neural Pathways: UNES-Prune’s Integrated Approach to Brain Tumor Segmentation and Classification ]"
