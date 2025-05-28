# 🧠 Project-2-NLP-Challenge_Group3

## 📌 Introduction  
This repository contains a Natural Language Processing (NLP) project aimed at developing a binary text classifier to distinguish between **real** and **fake news** based on article headlines and content. This challenge simulates a real-world task where preprocessing, model selection, and evaluation play a crucial role in building an effective NLP pipeline.

---

## 🗂️ Dataset  
The main training dataset is located in `dataset/data.csv` and includes the following columns:
- `label`: Target variable (0 = Fake News, 1 = Real News)  
- `headline`: News article headline (all in lowercase)

Additionally, `validation_data.csv` is provided for testing the final model. It contains news samples labeled as `2`, which must be replaced with predicted labels (`0` or `1`) using the trained classifier.

---

## 🎯 Objective  
Build and evaluate a machine learning model that can accurately predict whether a given news article is **real** or **fake**.  
Your final output should be a new version of `validation_data.csv` where all `label` values of `2` are replaced by predictions (`0` or `1`), preserving the original file structure.

---

## ⚙️ Workflow  

### 1. Data Cleaning & Preprocessing  
- Handle missing values  
- Apply text normalization (e.g., removing punctuation, stopwords, lowercasing, etc.)

### 2. Train-Test Split  
- Split `data.csv` into training and testing subsets

### 3. Model Building  
- Implement a pipeline using **TF-IDF**, **Bag of Words**, or other vectorizers  
- Use models like `LogisticRegression`, `RandomForestClassifier`, or others  
- Train the model on the training set

### 4. Model Evaluation  
- Evaluate performance on the test set using classification metrics such as accuracy, precision, recall, F1-score, and confusion matrix

### 5. Prediction on Validation Data  
- Use the trained model to predict labels in `validation_data.csv`  
- Replace `label` value `2` with predictions and save to `validation_data_predicted.csv`

### 6. Model Accuracy Prediction  
- Estimate the model's final accuracy based on validation or test set results and document confidence in predictions

### 7. Presentation  
- Prepare a PowerPoint presentation explaining:
  - The steps followed
  - Techniques used
  - Final results and conclusions

---

## 🛠️ Tools & Libraries  
- Python  
- pandas, NumPy  
- scikit-learn  
- nltk / spaCy (for text preprocessing)  
- matplotlib / seaborn (for visualization)
