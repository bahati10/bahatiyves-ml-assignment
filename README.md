# Titanic ML Assignment 🚢

This project is a full end-to-end data science pipeline on the Titanic dataset, following the structure required by the AI (ML) & Big Data assignment.

> Instructor: Lecturer. Victor Muvunyi  
> Submission Deadline: June 14, 2025  
> My GitHub Repo: https://github.com/bahati10/bahatiyves-ml-assignment

---

## 🔍 Objective

Build a machine learning pipeline from scratch using Python to predict survival on the Titanic. The pipeline includes:

- Data cleaning
- Exploratory data analysis (EDA)
- Machine learning modeling
- Interactive UI using Streamlit

---

## 📁 Project Structure

├── notebook.ipynb # Jupyter notebook with all tasks
├── app.py # Streamlit app for prediction (Task 4)
| ├── data # Cleaned Titanic dataset
| ├── cleaned_data.csv # Cleaned Titanic dataset
├── titanic.csv # Titanic dataset
├── titanic_model.pkl # Trained RandomForest model
├── model_columns.pkl # Feature list used in model
├── requirements.txt # Python dependencies
├── README.md # Project documentation
└── .gitignore # Files to ignore in version control

---

## 🧪 Task Breakdown

### ✅ Task 1: Data Cleaning

- Dataset: Titanic
- Tools: `pandas`
- Actions:
  - Handled missing values (`Age`, `Embarked`)
  - Dropped unnecessary columns (`Cabin`, `Name`, `Ticket`)
  - Saved cleaned data to `cleaned_data.csv`

---

### 📊 Task 2: Exploratory Data Analysis (EDA)

- Tools: `matplotlib`, `seaborn`, `ydata-profiling`
- Highlights:
  - Summary statistics (`df.describe(include='all')`)
  - Visualizations:
    - Survival countplot
    - Age distribution histogram
    - Heatmap of feature correlations

---

### 🤖 Task 3: Machine Learning Model

- Algorithm: `RandomForestClassifier`
- Tools: `scikit-learn`
- Workflow:
  - Encoded categorical variables (`Sex`, `Embarked`)
  - Trained/test split (80/20)
  - Evaluated using accuracy, classification report, and confusion matrix
  - Saved model using `joblib`

---

### 🖥️ Task 4: UI with Streamlit

- File: `app.py`
- Features:
  - Interactive form inputs (class, sex, age, fare, etc.)
  - Predicts survival using trained model
  - Displays result in browser with `st.success()` or `st.warning()`

---

## ⚙️ Setup Instructions

### 🔹 1. Clone the repo

```bash
git clone https://github.com/bahati10/bahatiyves-ml-assignment
cd bahatiyves-ml-assignment
```

### 🔹 2. Create a virtual environment (recommended)

```bash
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
```

### 🔹 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 🔹 4. Run Streamlit App

```bash
streamlit run app.py
```

### ✅ Requirements

### All dependencies are listed in requirements.txt, including:

- pandas

- seaborn

- matplotlib

- scikit-learn

- ydata-profiling

- streamlit

- joblib

### 📊 Sample Prediction

Enter details in the web form and get a prediction like:

```bash
🎉 Survived!
```

OR

```bash
❌ Did not survive.
```

### 📌 Notes

- Cleaned dataset: cleaned_data.csv

- Model saved as: titanic_model.pkl

- Make sure these files are in the root directory when running the app.

### 🧑‍💻 Author

Bahati Yves
ML Assignment for AI (ML) & Big Data
June 2025
