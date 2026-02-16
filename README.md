# Breast Cancer Artificial Perception System

This project develops an artificial perception system to classify breast tumors as **benign** or **malignant** using morphological features extracted from digitized biopsy images.  
The system learns patterns in nucleus size and boundary irregularity measurements to perform automated diagnosis.

The best model achieves **98.2% classification accuracy** on unseen test data and identifies clinically meaningful morphological predictors aligned with pathology knowledge.

---

## Models

The following machine learning models were trained and compared:

- Logistic Regression  
- Support Vector Machine (RBF)  
- Random Forest  
- Neural Network (MLP)  

**Best accuracy:** 98.2%

---

## Feature Importance

![Feature Importance](results/feature_importance.png)

Feature importance analysis shows that tumor **size** and **boundary irregularity** dominate classification decisions.  
Worst-case perimeter, area, and concave point measurements contribute most strongly, indicating reliance on the most atypical observed cell regions — consistent with clinical pathology characteristics of malignant tumors.

---

## Project Structure

data/ dataset
models/ trained model + scaler
results/ figures and metrics
src/ training and prediction code
notebooks/ exploration notebook


---

## Usage

Install dependencies:

pip install -r requirements.txt


Train the model:

python src/train.py


Predict on new patient data:

python src/predict.py


---

## Dataset

UCI Breast Cancer Wisconsin dataset containing **569 tumor samples** with **30 morphological features** derived from digitized fine-needle aspiration biopsy images of breast masses.

Features describe nucleus characteristics such as:

- radius  
- perimeter  
- area  
- concavity  
- concave points  
- texture  
- smoothness  

These measurements capture clinically relevant indicators of malignant growth.

---

## Results

- Test accuracy: **98.2%**
- Balanced precision and recall for both classes
- Dominant predictors: perimeter, area, radius, concavity
- Model learned medically meaningful morphology patterns

---

## Project Highlights

- Medical artificial perception system  
- Multi-model comparison framework  
- Explainable feature importance analysis  
- Deployment-ready trained model and scaler  
- Reproducible ML pipeline  

---

## Author

Aditya Kapile  
GitHub: https://github.com/Aditya-1711/breast-cancer-perception/)
