# CSE 572 – Data Mining

This repository contains my coursework for **CSE 572: Data Mining**.  
It includes homework assignments, code implementations, experiments, and analysis related to data preprocessing, classification, clustering, and evaluation techniques covered in the course.

The repository will be updated throughout the semester as new homework assignments are completed.

---

## Repository Structure

Each homework folder contains:
- Jupyter notebooks with code and analysis
- Any datasets used for the assignment
- A brief README explaining the task and approach (when applicable)

---

## Homework 1 – Classification on the Titanic Dataset

**Goal:**  
Apply multiple classification models and analyze the effect of data preprocessing on model performance.

**Models Implemented:**
- Support Vector Machines
- K-Nearest Neighbors
- Logistic Regression
- Random Forest
- Decision Tree
- Naive Bayes
- Perceptron
- Stochastic Gradient Descent
- Linear SVC

**Key Data Preprocessing Improvements:**
- Extracted meaningful features such as `Deck` from `Cabin`
- Added missing value indicators (e.g., `Age_missing`)
- Kept numerical features (Age, Fare) continuous instead of aggressive binning
- Applied log transformation to Fare to reduce outlier effects
- Used one-hot encoding for categorical variables like `Embarked` and `Title`
- Ensured train/test feature alignment after encoding

**Evaluation:**
- Initial model comparisons were done using training accuracy
- Cross-validation was later added to detect and explain overfitting
- Observed that tree-based models overfit the training data, while linear and distance-based models benefited most from improved preprocessing

---

## Tools & Libraries
- Python
- NumPy
- Pandas
- Scikit-learn
- Jupyter Notebook

---

## Notes
- This repository is for academic use as part of CSE 572.
- Code is written incrementally to reflect experimentation and learning.
- Future homework assignments will be added as separate folders.

---

## Author
Student, CSE 572 – Data Mining
