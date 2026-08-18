# Chest X-Ray Dataset Analysis

Exploratory analysis and preprocessing of a multi-label chest X-ray dataset.

## Overview

This project explores and prepares a chest X-ray dataset for multi-label image classification. The analysis focuses on understanding the metadata, diagnostic findings, patient distribution, class imbalance, image availability, and data quality.

## Dataset

The metadata contains:

- 111,010 X-ray records
- 30,538 unique patients
- 15 unique labels
- 14 chest findings and a `No Finding` label
- Multiple findings may be associated with a single X-ray

The provided image archive contains 3,710 PNG images.

After matching the image files with the ground-truth metadata:

- 3,681 images have valid matching labels
- 29 images do not have matching metadata
- The final usable dataset contains 3,681 labelled chest X-rays

## Analysis Performed

The notebook includes:

- Dataset extraction and loading
- Ground-truth metadata analysis
- Finding-label exploration
- Class distribution analysis
- Patient-level analysis
- Image availability validation
- Dataset cleaning
- Analysis of the usable image subset
- Chest X-ray visualisation
- Identification of unmatched images

## Key Observations

- The dataset is a multi-label classification dataset because one X-ray may contain multiple findings.
- The class distribution is highly imbalanced.
- Multiple X-rays may belong to the same patient.
- Patient-level separation should be considered when preparing data for machine-learning experiments to reduce data leakage.
- Only images with corresponding ground-truth metadata were retained in the usable dataset.

## Notebook

The complete analysis is available in:

`chest_xray_dataset_analysis.ipynb`

## Technologies

- Python
- Pandas
- Matplotlib
- Pillow
- Google Colab

## Disclaimer

This project is intended for educational and research purposes only. It is not intended for clinical diagnosis or medical decision-making.
