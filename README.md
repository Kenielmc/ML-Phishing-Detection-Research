
# Machine Learning Based Security Threat Detection:
## Robustness and Generalization

**Author:** Keniel Melesio Crespo  
**Institution:** University of Central Florida  
**Course:** CAP 5150  
**Semester:** Fall 2026

## Project Overview

This research examines the reliability of machine
learning models for phishing website detection.
The goal is to determine whether models that
perform well under normal testing conditions
maintain their performance when input features
are degraded or the data distribution changes.

## Machine Learning Models

- Random Forest
- Histogram Gradient Boosting

## Dataset

The project uses the phishing website dataset
developed by Vrbancic, Fister, and Podgorelec.

- Original samples: 88,647
- Cleaned samples: 87,209
- Input features: 111
- Training split: 80%
- Testing split: 20%
- Random seed: 42

Dataset source:
https://github.com/GregaVrbancic/Phishing-Dataset

## Methodology

The project consists of four main experiments:

1. Baseline performance evaluation
2. Robustness under simulated feature degradation
3. Generalization under URL-length dataset shift
4. Defense evaluation using data augmentation
   and feature removal

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- Balanced Accuracy
- False Positive Rate

## Repository Structure

- Phishing_Detection_Research.ipynb:
  Complete Python implementation.
- results/:
  Numerical experimental results in CSV format.
- figures/:
  Performance graphs and confusion matrices.

## How to Run

1. Download the phishing dataset from its source.
2. Open the notebook in Google Colab.
3. Upload the dataset to the Colab environment.
4. Ensure the CSV filename matches the notebook.
5. Run all notebook cells in order.

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

## Limitations

The robustness experiment uses simulated feature
degradation rather than real-world adversarial
attacks. Generalization is evaluated using a
URL-length-based distribution shift within a
single dataset. Therefore, the results do not
establish robustness against all attacks or
generalization to independent datasets.

## Purpose

This repository contains the implementation and
experimental artifacts supporting the final
research paper for CAP 5150 at the University
of Central Florida.
