# Credit Card Fraud Detection Analysis

This project analyzes a dataset of credit card transactions to detect fraudulent activity. Due to the highly imbalanced nature of the dataset (fraudulent transactions are very rare), this notebook utilizes **Exploratory Data Analysis (EDA)** and **SMOTE (Synthetic Minority Over-sampling Technique)** to balance the data before training machine learning models.

## 📂 Files

- `test.ipynb`: The main Jupyter Notebook containing data loading, visualization, and analysis logic.
- `requirements.txt`: List of Python dependencies required to run the notebook.
- `creditcard.csv`: **(Not included in repo)** The dataset file. See the "Dataset" section below for download instructions.

## 🚀 Setup & Installation

1.  **Clone or download** this repository.
2.  **Install the required libraries** using pip:

    ```bash
    pip install -r requirements.txt
    ```

3.  **Download the Data**: Follow the instructions in the [Dataset](#-dataset) section to get the `creditcard.csv` file.
4.  **Launch Jupyter Notebook**:

    ```bash
    jupyter notebook
    ```

5.  Open `test.ipynb` to view and run the analysis.

## 📊 Dataset

The dataset used in this project is the **Credit Card Fraud Detection** dataset. It is not included in this repository because it exceeds GitHub's file size limits.

**You must download the dataset manually:**

1.  Go to the Kaggle dataset page: [https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
2.  Download the `creditcard.csv` file.
3.  Place the file in the **root directory** of this project (the same folder as `notebook.ipynb`).

## 🧠 Project Workflow

1.  **Data Loading**: Reading the transaction data.
2.  **Exploratory Data Analysis (EDA)**:
    - Checking for missing values.
    - Visualizing the class imbalance (Fraud vs. Normal).
    - Analyzing statistics of transaction amounts.
3.  **Preprocessing (Planned)**:
    - Scaling features (e.g., 'Amount' and 'Time').
    - Splitting data into Training and Testing sets.
4.  **Handling Imbalance**:
    - Applying **SMOTE** (Synthetic Minority Over-sampling Technique) to the training data to generate synthetic fraud samples.
5.  **Modeling & Evaluation**:
    - Training classifiers (e.g., XGBoost, Logistic Regression).
    - Visualizing performance using **Confusion Matrices** and classification reports.

## 🛠 Libraries Used

- **Pandas & NumPy**: For data manipulation and numerical operations.
- **Matplotlib & Seaborn**: For plotting graphs and heatmaps.
- **Imbalanced-learn**: For applying SMOTE.
- **Scikit-learn**: For model training and evaluation metrics.
