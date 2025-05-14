
# ECE7123 Deep Learning Project 3
This repository contains the project submission for "Deep Learning Project 3: Jailbreaking Deep Models," focusing on adversarial attacks against image classifiers, especially ResNET-34.

## Project Overview

The project explores the vulnerability of a pre-trained ResNet-34 model to various adversarial attack techniques on a subset of the ImageNet dataset. We implement and evaluate:
*   **Pixel-wise $L_\infty$ attacks:** FGSM, PGD, MIM (with $\epsilon=0.02$)
*   **Patch-based $L_\infty$ attacks:** Targeted MIM Patch, Saliency-Guided MIM Patch, LaVAN-style Patch (32x32 patches with $\epsilon=0.5$)

The effectiveness of these attacks is measured by the degradation in Top-1 and Top-5 accuracy on ResNet-34. Additionally, the transferability of the generated adversarial examples to an EfficientNet-B0 model is assessed.

## Repository Contents

*   **`finalproject_v0.ipynb`**: The main Jupyter Notebook containing all code for:
    *   Loading datasets and models.
    *   Implementation of all adversarial attack methods.
    *   Evaluation of attacks on ResNet-34.
    *   Transferability tests on EfficientNet-B0.
    *   Generation of all figures and detailed result tables.
    *   **Note:** The notebook provides a comprehensive record of all methods explored and their detailed outputs. Some granular details or intermediate results might be present in the notebook but were summarized or excluded from the final PDF report due to length constraints. The report focuses on the most salient findings and best-performing methods.
*   **`DLFinalProject.pdf`**: A PDF version of the Jupyter Notebook, provided as a stable alternative in case the `.ipynb` file fails to render correctly on GitHub.

## Key Findings

*   MIM was the most potent full-image attack against ResNet-34.
*   LaVAN-style patch attacks were highly effective among localized attacks.
*   Adversarial examples demonstrated transferability to EfficientNet-B0, though with varying degrees of reduced effectiveness.

For a detailed analysis and discussion, please refer to the Jupyter Notebook.
