# Breast-Cancer-Classification-using-Support-Vector-Machines-Task-7-

> This project applies **Support Vector Machines (SVM)** with both **linear** and **RBF kernels** to classify breast cancer cases as malignant or benign using the Breast Cancer Wisconsin dataset.

---

## 📁 Dataset
- Source: Breast Cancer Wisconsin Dataset (`data.csv`)
- Target: `diagnosis` (M = Malignant, B = Benign)
- Features: Radius, texture, perimeter, area, smoothness, etc.

---

## 🎯 Objectives
- Apply linear and non-linear SVM models
- Visualize decision boundaries using 2D feature combinations
- Tune hyperparameters (`C`, `gamma`) using GridSearchCV
- Evaluate model using confusion matrix, accuracy, and cross-validation

---

## 🧰 Tools Used
| Tool         | Purpose                         |
|--------------|----------------------------------|
| Python       | Programming Language             |
| Pandas       | Data manipulation                |
| Scikit-learn | Modeling, preprocessing, tuning  |
| Seaborn      | Visualizations                   |
| Matplotlib   | Plotting                         |

---

## 🔄 Workflow

1. **Data Loading and Cleaning**
    - Removed unnecessary columns (`id`, `Unnamed: 32`)
    - Encoded target column (`diagnosis`: M → 1, B → 0)

2. **Feature Scaling**
    - Used `StandardScaler` to normalize input features

3. **Model Training**
    - Trained Linear SVM (`kernel='linear'`)
    - Trained RBF SVM (`kernel='rbf'`)

4. **Evaluation**
    - Accuracy, confusion matrix, and classification report
    - Cross-validation scores

5. **Hyperparameter Tuning**
    - Used `GridSearchCV` to find best `C` and `gamma` for RBF

6. **Decision Boundary Visualization**
    - Used two features (radius & perimeter) to illustrate margin

---

## 📊 Key Visuals

- Linear SVM decision boundary (2D plot)
- RBF decision boundary
- Confusion matrix and CV performance

---

## 💡 Key Learnings

- **Linear SVM** is interpretable and works well with linearly separable data.
- **RBF SVM** handles more complex boundaries better.
- `C` controls the margin size and regularization.
- `gamma` defines how far the influence of a single training point reaches in RBF kernel.
- Normalization is essential for distance-based algorithms like SVM.

---

## 📂 Folder Structure

📁 svm-breast-cancer
│
├── data.csv # Dataset
├── task7_svm_classifier.py # Python script
├── README.md # This file

---

## 🚀 How to Run
1. Place your dataset in the project directory as `data.csv`
2. Install dependencies:
pip install pandas scikit-learn matplotlib seaborn
3. Run the script:
