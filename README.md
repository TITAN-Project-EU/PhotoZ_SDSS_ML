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

### MLP classification

The  [Python script](MLP_PhotoZ_SDSS.ipynb) demonstrates the complete process of using photometric data from the Sloan Digital Sky Survey (SDSS) to predict the redshift of galaxies using a machine learning model. The script includes data loading, preprocessing, visualization, model training, evaluation, and saving. It utilizes the TensorFlow library to construct and train a Multi-Layer Perceptron (MLP) neural network.
