# Galaxy Redshift Prediction

This project utilizes data from the Sloan Digital Sky Survey (SDSS) to create a machine learning model that predicts the redshift of galaxies based on their photometric properties ('u', 'g', 'r', 'i', 'z'). The model is built using TensorFlow, demonstrating the application of a Multi-Layer Perceptron (MLP) in predicting astronomical measurements.

## Project Overview

The dataset comprises photometric properties and redshifts for approximately 1M galaxies, with the aim of training a machine learning model to understand and predict how these properties correlate with redshift. The model could potentially be used to estimate redshifts for other astronomical data, assisting in cosmological studies.

## Data Description

The data is extracted using a SQL query from the SDSS online database, which includes:
- Photometric magnitudes in five different bands (u, g, r, i, z).
- Spectroscopic redshifts and their errors.
- Metadata such as right ascension (ra), declination (dec), and object identifiers.

## Getting Started

Download data from Zenodo  
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11073039.svg)](https://doi.org/10.5281/zenodo.11073039)

### Dependencies

Ensure you have the following installed:
- Python 3.8 or above
- TensorFlow 2.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

### MLP Regression and Classification

The Python notebooks demonstrate the complete process of using photometric data from the Sloan Digital Sky Survey (SDSS) to predict the redshift of galaxies using machine learning techniques.

The redshift prediction problem is explored under **two formulations**:
-  [**Regression**](MLP_PhotoZ_SDSS.ipynb), where the redshift is treated as a continuous variable and predicted directly using a Multi-Layer Perceptron (MLP).
-  [**Classification**](MLP_PhotoZ_SDSS_R&C.ipynb), where the redshift range is discretized into bins, and the model is trained to classify galaxies into redshift intervals (also includes the regression case above)

Both models are evaluated and compared in terms of predictive accuracy and error metrics, offering insights into the effectiveness of each approach.
