# K-Fold Cross Validation from Scratch using NumPy

## 📌 Overview

This project implements **K-Fold Cross Validation from scratch** using only **NumPy**. The goal is to understand how K-Fold Cross Validation works internally without using Scikit-learn's `KFold` or `cross_val_score`.

A **Linear Regression model** is trained using the **Normal Equation** on each training fold, and the **Mean Squared Error (MSE)** is computed on the corresponding test fold. The final performance is obtained by averaging the MSE across all folds.

---

## 🚀 Features

- K-Fold Cross Validation implemented from scratch
- User-defined number of folds (K)
- Automatic train/test split for each fold
- Linear Regression using the Normal Equation
- Mean Squared Error (MSE) calculation for each fold
- Average MSE across all folds
- Implemented using only NumPy

---

## 🛠 Technologies Used

- Python
- NumPy
- Google Colab / Jupyter Notebook

---

## 📂 Project Structure

```
KFold-Cross-Validation-From-Scratch/
│
├── KFold_Cross_Validation.ipynb
├── README.md
└── requirements.txt
```

---

## 📖 How It Works

1. Load the dataset.
2. Split the dataset into **K** equal folds.
3. Repeat for each fold:
   - Use one fold as the test set.
   - Use the remaining folds as the training set.
   - Train a Linear Regression model using the Normal Equation.
   - Predict on the test set.
   - Calculate the Mean Squared Error (MSE).
4. Compute the average MSE across all folds.

---

## 📊 Example Output

```
Enter number of folds: 5

Fold 1 MSE: 0.0
Fold 2 MSE: 0.0
Fold 3 MSE: 0.0
Fold 4 MSE: 0.0
Fold 5 MSE: 0.0

Average MSE:
1.4199496293978212e-29
```

The extremely small value (`1.42 × 10⁻²⁹`) is due to floating-point precision and is effectively equal to zero.

---

## 🎯 Learning Objectives

This project helped me understand:

- How K-Fold Cross Validation works internally
- Manual dataset splitting using NumPy
- Training multiple models on different folds
- Model evaluation using Mean Squared Error (MSE)
- Linear Regression using the Normal Equation
- Why Cross Validation provides a more reliable estimate of model performance

---

## 🔮 Future Improvements

- Implement Gradient Descent instead of the Normal Equation
- Support Multiple Linear Regression
- Add R² Score
- Support custom evaluation metrics
- Compare results with Scikit-learn
- Add visualization of fold splits

---

## 📜 License

This project is open-source and available under the MIT License.
