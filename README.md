# Brain Tumor Classification using GAN

## Project Overview
This project applies Deep Learning techniques to classify brain tumors into three specific categories: **Glioma**, **Meningioma**, and **Pituitary tumor**. 
First I implement the authors methodology of augmenting the images, and their deep learning model.
I then try to optimize the baseline results as their previous method gave us poor results.
Then I implements a **Wasserstein GAN (WGAN)** for data augmentation to enhance the dataset and compares a baseline classification model against an optimized version.

## Repository Structure
**IMPORTANT:** This project relies on relative paths. Please ensure the following directory structure is maintained exactly as shown below when running the notebook. Do not move the folders or the notebook file.

## Disclaimer - Install the specific version of the libraries as given in requirement.txt - before running the code.
## Please keep the folder paths as per submission - no change is required.

The folder - file structure has been given below:

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
