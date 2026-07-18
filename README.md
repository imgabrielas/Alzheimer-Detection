# Alzheimer's Disease Detection using Machine Learning

A machine learning project exploring Alzheimer's disease classification using MRI volumetric measurements, cognitive assessment scores, and clinical information. The project demonstrates a complete end-to-end machine learning workflow, including data preprocessing, feature engineering, model training, and evaluation.

---

## Project Overview

The goal of this project is to classify patients based on Alzheimer's disease diagnosis by combining data from multiple clinical datasets. The notebook focuses on preparing real-world medical data for machine learning and evaluating a classification model.

The workflow includes:

- Data cleaning
- Missing value handling
- Merging multiple datasets
- Feature scaling
- Categorical encoding
- Feature selection
- Model training
- Model evaluation

---

## Dataset

The project combines three datasets:

- **MRI volumetric measurements**
- **Cognitive assessment scores**
- **Clinical diagnosis data**

The datasets are merged using the patient identifier (`RID`) to create a single dataset for machine learning.

---

## Data Preprocessing

The preprocessing pipeline includes:

- Removing unnecessary columns
- Converting incorrect data types
- Handling missing values
  - Mean imputation for selected numerical features
  - Removing remaining missing observations
- Converting categorical variables using **One-Hot Encoding**
- Standardizing numerical features using **StandardScaler**
- Merging datasets into a unified DataFrame

---

## Machine Learning Pipeline

The notebook follows a standard supervised learning workflow:

1. Load datasets
2. Clean and preprocess data
3. Merge datasets
4. Separate features (`X`) and target (`y`)
5. Encode categorical variables
6. Scale numerical features
7. Split into training and testing sets
8. Train the classification model
9. Evaluate model performance

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook

---

## Results

The initial model achieved:

| Metric | Score |
|---------|------:|
| Training Accuracy | **100%** |
| Testing Accuracy | **50%** |

The significant difference between training and testing accuracy indicates **overfitting**. While the model learned the training data extremely well, it did not generalize successfully to unseen examples.

This project therefore serves as an exploration of the machine learning workflow rather than a final optimized predictive model.

---

## Future Improvements

Possible directions for improving performance include:

- Hyperparameter tuning
- Cross-validation
- Testing additional classification algorithms
- Feature selection
- Dimensionality reduction (PCA)
- Better handling of class imbalance
- Additional feature engineering
- Larger and more diverse datasets

---

## Repository Structure

```text
.
├── data/
│   ├── cognitive.csv
│   ├── data.csv
│   └── diagnosis.csv
│
├── notebooks/
│   └── alzheimer_detection.ipynb
│
├── README.md
└── requirements.txt
```

---

## Key Takeaways

This project demonstrates an end-to-end machine learning workflow for medical data, from preprocessing and feature engineering to model evaluation. Although the first model exhibited overfitting, the notebook provides a solid foundation for experimenting with more advanced techniques and improving predictive performance.

---

*This project was created for educational and portfolio purposes.*****# Alzheimer-Detection
