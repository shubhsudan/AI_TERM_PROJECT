# Brain Tumor Classification using WGAN

##  Project Overview
This project applies Deep Learning techniques to classify brain tumors into three specific categories: **Glioma**, **Meningioma**, and **Pituitary tumor**.

The project methodology proceeds in three key stages:
1.  **Baseline Implementation:** Implementing the original authors' methodology for image augmentation and their deep learning model.
2.  **Optimization:** Optimizing the baseline architecture and hyperparameters to address performance limitations observed in the initial method.
3.  **WGAN Augmentation:** Implementing a **Wasserstein GAN (WGAN)** to generate synthetic data, enhancing the dataset to further improve the robustness of the optimized model.

##  Disclaimer
> **Crucial Setup Instructions:**
> * **Library Versions:** You must install the specific versions of the libraries listed in `requirements.txt` before running the code to avoid compatibility errors.
> * **Directory Structure:** Please maintain the folder paths exactly as submitted. No changes to the file structure are required or recommended.

## Repository Structure
**IMPORTANT:** This project relies on relative paths. Please ensure the following directory structure is maintained exactly as shown below when running the notebook.

```text
AI_TERM_PROJECT/
│
├── AI_TERM_PROJECT.ipynb        # Main Jupyter Notebook containing training & evaluation code
├── requirements.txt             # List of all Python library dependencies
├── sultan_optimized_best.keras  # Saved model (Optimized version)
├── sultan_paper_baseline.keras  # Saved model (Baseline version)
│
├── data/                        # Original source dataset
│   ├── Glioma/
│   ├── Meningioma/
│   └── Pituitary tumor/
│
├── augmented_images/            # Synthetic data generated via WGAN
│   ├── train/
│   └── test/
│
├── WGAN_Results/                # WGAN training outputs and visualizations
│   ├── Glioma/
│   ├── Meningioma/
│   └── Pituitary tumor/
│
└── checkpoints/                 # Training checkpoints for the models
