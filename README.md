# Breast Cancer Classification Using Support Vector Machine (SVM)

## Project Overview
This project uses a Support Vector Machine (SVM) machine learning algorithm to classify breast cancer tumors as **malignant** or **benign** using the Breast Cancer Wisconsin dataset from scikit-learn.

## Dataset
- **Samples:** 569
- **Features:** 30 numerical features
- **Classes:** Malignant and Benign
- **Training samples:** 455
- **Testing samples:** 114

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Joblib

## Machine Learning Workflow
1. Loaded and explored the dataset.
2. Analyzed target class distribution.
3. Split the data into training and testing sets.
4. Standardized features using `StandardScaler`.
5. Trained an SVM classifier.
6. Evaluated predictions using accuracy, a classification report, and a confusion matrix.
7. Tuned hyperparameters using `GridSearchCV` with 5-fold cross-validation.
8. Saved the tuned model using Joblib.
9. Loaded the saved model and tested predictions.

## Results
- **Original SVM test accuracy:** 98.25%
- **Tuned SVM test accuracy:** 98.25%
- **Best cross-validation accuracy:** 97.80%
- **Best kernel:** Linear
- **Best C:** 0.1
- **Best gamma:** `scale`

Hyperparameter tuning did not improve the test accuracy, but the tuned model achieved the same accuracy as the original model.

## Project Structure
```text
svm-breast-cancer-classification-new/
├── models/
│   └── svm_breast_cancer_model.pkl
├── svm_classification.ipynb
└── README.md
```

## How to Run
1. Install Python and the required libraries.
2. Open `svm_classification.ipynb` in VS Code or Jupyter Notebook.
3. Select a Python kernel with the required packages installed.
4. Run the notebook cells in order.

Install the main dependencies with:

```bash
python -m pip install numpy pandas matplotlib seaborn scikit-learn joblib ipykernel
```

## Disclaimer
This project is for educational purposes only. It is not a medical diagnostic tool and must not be used to make real-world medical decisions.
