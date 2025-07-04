# 📩 Spam SMS Detection — CodSoft Internship Task 4

This project involves building a machine learning model to classify SMS messages as either **Spam** or **Ham (Legitimate)** using natural language processing (NLP) techniques. The goal is to prevent spam messages from reaching users by training and evaluating multiple classifiers on a labeled dataset.


## 🔍 Problem Statement

With the increasing volume of mobile text communication, detecting spam SMS is crucial to ensure security and user trust. This project applies classical machine learning algorithms combined with text feature extraction techniques to develop a reliable spam detection system.


## 🛠️ Technologies Used

Python
Pandas, NumPy
Scikit-learn
Matplotlib, Seaborn
TF-IDF (Term Frequency - Inverse Document Frequency)
NLP preprocessing
Classification Models:
  Naive Bayes
  Logistic Regression
  Support Vector Machine (SVM)


## 🧪 Workflow

1. **Data Preprocessing**:
   - Removed null columns
   - Encoded labels: 'ham' → 0, 'spam' → 1
   - Normalized text data

2. **Vectorization**:
   - Used TF-IDF to convert SMS text to numerical vectors

3. **Model Training**:
   - Trained Naive Bayes, Logistic Regression, and SVM on the vectorized dataset

4. **Evaluation**:
   - Evaluated using accuracy, precision, recall, F1-score, and confusion matrix


## 📊 Results & Insights

 Model                Accuracy  Precision (Spam)  Recall (Spam)  F1-Score (Spam) 

 Naive Bayes          0.98      0.95              0.97            0.96            
 Logistic Regression  0.98      0.96              0.95            0.95            
 SVM                  0.99      0.98              0.98            0.98            

### ✅ Insights:
* **SVM performed the best** in all metrics, especially in minimizing false positives (ham predicted as spam).
*  **Naive Bayes**, although simpler, gave very strong results due to its effectiveness on word probability distributions.
*  TF-IDF vectorization greatly improved model performance compared to simpler count methods.


## 📁 Dataset
* Used the classic `spam.csv` dataset available on Kaggle and UCI repository.
8 Contains ~5,500 labeled SMS messages with categories: `spam` and `ham`.


## 📌 How to Run

```bash
# Install required libraries
pip install pandas scikit-learn matplotlib seaborn

# Run the main Python script
python spam_sms_detection.py

```
