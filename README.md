# 🍄 Mushroom Toxicity Classification using scikit-learn

This project focuses on classifying mushrooms as toxic or non-toxic using various machine learning models. The dataset is processed and analyzed in a Jupyter Notebook, and the best-performing model is used to predict toxicity on unseen data.

## 📁 Dataset

The project uses two input files:

- `input.csv` – training data
- `validation.csv` – data to predict toxicity for

## ⚙️ Preprocessing

The following preprocessing steps were applied:

- Categorical columns were converted to numeric using `pd.factorize`
- Missing values were filled with column medians
- Outliers were removed (e.g. filtering extreme values in `stem-height`)
- Selected features:  
  `cap-diameter`, `stem-height`, `stem-width`, `shape`, `type`, `ring`, `color`

## 🤖 Models Used

Several machine learning models were tested and compared based on accuracy:

- K-Nearest Neighbors (KNN) ✅ *(best accuracy: ~95.3%)*
- Decision Tree
- Bagging
- Random Forest 
- AdaBoost

The model with the highest accuracy was used to generate predictions on the `validation.csv` dataset.

## 📄 Output

Predictions are saved into the file: pred.txt

Each line contains the predicted class label for the corresponding row in `validation.csv`.

## 🧪 How to Run

1. Open `beadando.ipynb` in Jupyter Notebook or VS Code.
2. Make sure `input.csv` and `validation.csv` are in the same folder.
3. Run the notebook cell by cell.
4. At the end, predictions will be saved to `pred.txt`.

## 📦 Requirements

Make sure the following Python packages are installed:

```bash
pandas
numpy
scikit-learn
matplotlib
```

To install them: 
```bash
pip install pandas numpy scikit-learn matplotlib
```

## Author

Bálint Krisztián Keller

Computer Science BSc student

Interested in data science
