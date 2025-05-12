# Sentiment Analysis of IMDB Reviews 🎥

This is **Task 2** of my Data Science Internship at DevelopersHub Corporation.

The goal of this project is to build a **sentiment analysis model** that can tell whether a movie review is **positive** or **negative**, using the **IMDB Reviews dataset**.

---

## 📁 Dataset Used

I used the **IMDB Dataset of 50K Movie Reviews** from Kaggle.  
👉 [Click here to view the dataset on Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)
## 📁 Kaggle Notebook link 
👉 [Click here to view the noteboook on Kaggle](https://www.kaggle.com/code/ashirzaki/sentiment-analysis-ipynb)

---

## 📘 Steps I Followed

### 1. Loading the Data
- I loaded the dataset into a Pandas DataFrame.

### 2. Text Preprocessing
- Converted all text to lowercase
- Removed stopwords (like "the", "is", "and")
- Lemmatized each word to its base form
- Cleaned out symbols and HTML tags

### 3. Feature Engineering
- Used **TF-IDF** to convert text into numeric values the model can understand.

### 4. Model Training
- I trained a **Logistic Regression** model to classify the review as either **Positive (1)** or **Negative (0)**.

### 5. Evaluation
- I tested the model using:
  - **Accuracy**
  - **Precision**
  - **Recall**
  - **F1-score**

### 6. Sample Prediction
- You can input any review text and get the model's prediction using a function:
```python
predict_sentiment("I loved this movie!")
# Output: Positive
