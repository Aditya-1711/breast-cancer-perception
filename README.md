# Breast Cancer Artificial Perception System

This project builds an artificial perception system to classify breast tumors as benign or malignant using morphological features extracted from digitized biopsy images.

## Models
- Logistic Regression  
- Support Vector Machine  
- Random Forest  
- Neural Network  

**Best accuracy:** 98.2%

## Feature Importance

![Feature Importance](results/feature_importance.png)

Feature importance analysis shows that tumor size and boundary irregularity dominate classification decisions. Worst-case perimeter, area, and concave point measurements contribute most strongly, indicating reliance on the most atypical observed cell regions.

## Project Structure

## Usage

Install dependencies:


Train model:


Predict on new data:


## Dataset

UCI Breast Cancer Wisconsin dataset containing 569 tumor samples with 30 morphological features derived from digitized biopsy images.


