# Spam Detection using Multinomial Naive Bayes

This repository contains a Machine Learning project that classifies text messages as **`spam`** or **`not spam`** using the **Multinomial Naive Bayes** algorithm. The text features are extracted using `CountVectorizer` (Bag-of-Words approach).

---

## 📌 Features

* **Text Preprocessing & Feature Extraction:** Converts text data into numerical vectors using `CountVectorizer`.


* **Classification Model:** Trains a `MultinomialNB` classifier from `scikit-learn`.


* **Performance Evaluation:** Evaluates model performance on unseen test data with an accuracy score of **~93.33%**.


* **Prediction Comparison:** Compares ground truth labels (`Actual`) against model outputs (`Predicted`).



---

## 🛠️ Requirements & Dependencies

Ensure you have Python installed along with the following packages:

* `pandas`

* `scikit-learn`


You can install the dependencies via pip:

```bash
pip install pandas scikit-learn

```

---

## 📂 Dataset

The project relies on a CSV file named **`MultinomialNB.csv`**.

* **Total Rows:** 600 text samples


* **Columns:**
* `text`: The string content of the message.


* `label`: Class label (`spam` / `not spam`).





---

## 🚀 Workflow & Code Execution

1. **Data Loading:** Load the dataset using Pandas dataframe.


2. **Train-Test Split:** Split the dataset into 80% training data and 20% testing data using `train_test_split` with `random_state=42`.


3. **Text Vectorization:** Transform textual data to token count matrices using `CountVectorizer`.


4. **Model Training:** Fit the `MultinomialNB` model on `x_train_vec` and `y_train`.


5. **Model Evaluation:** Generate predictions on test features `x_test_vec` and measure accuracy via `accuracy_score`.



---

## 📊 Results

* **Model Accuracy:** `93.33%`

* **Sample Output Comparison:**

| Index | Text | Actual | Predicted |
| --- | --- | --- | --- |
| 110 | team report urgent now details meeting | not spam | not spam |
| 419 | details win now prize free regarding | spam | spam |
| 565 | cash please now prize check update | spam | spam |
| 77 | now meeting please details about | not spam | not spam |

---

## 💻 How to Run

1. Place `MultinomialNB.csv` in the project root directory.


2. Launch and run the Jupyter Notebook file:

```bash
jupyter notebook

```
