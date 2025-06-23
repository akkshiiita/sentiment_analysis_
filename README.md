# 🧥 Women's Clothing E-Commerce Review Sentiment Analysis

This project analyzes customer reviews from a women's clothing e-commerce platform to extract insights and build sentiment classification models using machine learning and NLP.

## Dataset

The dataset used is the **Women's Clothing E-Commerce Reviews**, which contains:

* Customer reviews
* Ratings
* Recommendation status
* Feedback count
* Product metadata (division, department, etc.)

## Exploratory Data Analysis

We performed:

* Null value treatment and cleaning
* Distribution of Ratings and Recommendation Indicator
* Review length analysis by recommendation status
* Positive feedback and average rating by clothing ID
* Word clouds for high and low rated reviews

## Text Preprocessing

* Lowercasing, punctuation and number removal
* Lemmatization using `WordNetLemmatizer`
* TF-IDF Vectorization (max 5000 features)

## Sentiment Labeling

* **Positive**: Ratings 4–5
* **Neutral**: Rating 3
* **Negative**: Ratings 1–2

##  Models Used

We tested the following ML models:

| Model               | Pre-SMOTE Accuracy | Post-SMOTE Accuracy |
| ------------------- | ------------------ | ------------------- |
| Logistic Regression | ✅                  | ✅                   |
| Naive Bayes         | ✅                  | ✅                   |
| SVM (LinearSVC)     | ✅                  | ✅                   |
| Random Forest       | ✅                  | ✅                   |
| K-Nearest Neighbors | ✅                  | ✅                   |

> SMOTE was applied to handle class imbalance in sentiment labels.

##  Sample Prediction

Example:

```python
sample = ["The fit and fabric were good. Very happy."]
```

➡️ Model Output: **Positive**

## Libraries Used

* pandas, numpy
* matplotlib, seaborn, wordcloud
* nltk (stopwords, lemmatization)
* scikit-learn (LogisticRegression, SVM, etc.)
* imblearn (SMOTE)

## Visualizations

* Bar charts for rating and recommendation distribution
* Word clouds for positive and negative reviews
* Histograms of review length vs. recommendation

## Future Work

* Integrate a recommendation engine
* Streamlit web app for live sentiment prediction
* Hyperparameter tuning for better accuracy

---


