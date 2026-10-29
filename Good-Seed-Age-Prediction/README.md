# Good Seed — Age Prediction with Computer Vision

## Project Overview

This project explores the use of computer vision and deep learning to estimate customers' ages from facial images. The business objective is to support Good Seed, a supermarket chain, in monitoring compliance with alcohol sales regulations.

## Objectives

- Explore and analyze a dataset of facial images.
- Examine the age distribution of the individuals in the dataset.
- Develop a convolutional neural network (CNN) to estimate age.
- Evaluate model performance using regression metrics.

## Methodology

- **Exploratory Data Analysis:** Analyzed the age distribution and visualized sample images.
- **Image Processing:** Prepared image data using TensorFlow and ImageDataGenerator.
- **Model Development:** Implemented a CNN based on the ResNet50 architecture, using GPU training.
- **Model Evaluation:** Assessed performance using Mean Absolute Error (MAE) and Mean Squared Error (MSE).

## Results

- **Model architecture:** ResNet50-based CNN
- **Training MAE:** 3.30 years
- **Validation MAE:** 7.33 years
- **Validation MSE:** 89.03

## Tools & Technologies

Python · Pandas · NumPy · Matplotlib · PIL · TensorFlow · Keras · ResNet50

## Key Skills

Computer Vision · Image Processing · Deep Learning · Convolutional Neural Networks (CNN) · Transfer Learning · Model Evaluation

## Business Outcome

The model demonstrated the potential to estimate customer age from facial images and could support age-screening processes at checkout. However, automated age estimation should complement, not replace, official ID verification when checking compliance with alcohol sales regulations.

## Project Files

- `Age_verification.ipynb` — Notebook containing image exploration, preprocessing, model training, and evaluation.

## How to View

Open `Age_verification.ipynb` in GitHub to explore the analysis, code, and model evaluation. The notebook is written in Spanish.
