# 🌳 Decision Tree Classifier – Customer Purchase Prediction  
**Akanksha Bhosle | Data Science Intern @ Credora**

---

## 📌 Task Overview

In this task, I built a **Decision Tree Classifier** to predict whether a customer will subscribe to a term deposit based on their personal and banking information. The dataset was sourced from the UCI Machine Learning Repository and contains both categorical and numerical features.

---

## 📂 Dataset Description

**Source:** [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/dataset/222/bank+marketing)

**Files Used:**
- `bank.csv`: 10% sample of the full dataset (4,521 records)
- `bank-full.csv`: Complete dataset (45,211 records)
- `bank-names.txt`: Feature descriptions and attribute information

---

## 🧹 Data Cleaning & Preprocessing

- Loaded and compared both sample and full datasets
- No null values present, but multiple categorical features
- Encoded all categorical variables using `LabelEncoder`
- Split data into training and testing sets using `train_test_split`

---

## 🌳 Model: Decision Tree Classifier

- Trained a Decision Tree using `sklearn.tree.DecisionTreeClassifier`
- Limited depth to avoid overfitting (`max_depth=5`)
- Evaluated model using:
  - Accuracy Score
  - Confusion Matrix (Seaborn heatmap)
  - Classification Report (precision, recall, F1-score)

---

## 📈 Visualizations

- Confusion matrix to understand classification performance
- Full decision tree plotted using `plot_tree()` from sklearn
- Dataset structure and correlation explored visually

---

## 💡 Key Insights

- Dataset contains significant class imbalance (most customers did not subscribe)
- Features like **`duration`, `contact`, and `month`** had notable predictive power
- Decision tree showed strong interpretability for business decisions

---

## ⚠️ Challenges & Solutions

| Challenge | Solution |
|----------|----------|
| Multiple categorical features | Used `LabelEncoder` to convert to numeric |
| Decision tree overfitting | Limited `max_depth` and used pruning |
| Choosing between sample/full dataset | Used sample (`bank.csv`) for fast testing; full (`bank-full.csv`) for final training |

---

## 🛠️ Tools & Libraries

- Python  
- Pandas, NumPy  
- Scikit-learn (`DecisionTreeClassifier`, metrics, preprocessing)  
- Seaborn & Matplotlib (visualizations)  
- Google Colab

---

## 🔗 Project Links

- 📓 [Google Colab Notebook](https://colab.research.google.com/drive/1K0e8pLNscHsNqsSHPOKehOdl3D4rR_SD#scrollTo=-1I3lU_Sbf_F)  
- 💻 [GitHub Repository](https://github.com/akanksha21-maker/CREDORA-TASK-3)

---

## 📬 Contact

- **Name:** Akanksha Bhosle  
- **Email:** *akanshabhosle31@gmail.com*  
- **LinkedIn:** [linkedin.com/in/akanksha-bhosle](https://www.linkedin.com/in/akanksha-bhosle)

---

> “A good model tells a story. A great one tells you why.”  
> — Task 3 complete 🚀
