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

### Dependencies

Ensure you have the following installed:
- Python 3.8 or above
- TensorFlow 2.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

You can install the necessary Python libraries using pip:

```bash
pip install tensorflow pandas numpy scikit-learn matplotlib
