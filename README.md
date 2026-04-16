# Amazon Alexa Sentiment Analysis using Machine Learning

## Project Overview
This project performs **sentiment analysis** on Amazon Alexa product reviews. The goal is to classify customer feedback as **positive or negative** using Natural Language Processing (NLP) and Machine Learning techniques.

The project demonstrates the full ML pipeline including:
- Data preprocessing
- Feature engineering
- Model training (Random Forest)
- Model evaluation
- Prediction on new data

## Dataset
- Source: Kaggle (Amazon Alexa Reviews Dataset)
- Size: ~3000 customer reviews
- Features:
  - `rating`: Product rating (1–5)
  - `date`: Review date
  - `variation`: Product type
  - `verified_reviews`: Review text
  - `feedback`: Sentiment (1 = Positive, 0 = Negative)

## Technologies Used
- Python
- Google Colab
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

## Methodology

### 1. Data Preprocessing
- Removed irrelevant columns (`date`, `rating`)
- One-hot encoding applied to `variation`
- Cleaned and tokenized review text

### 2. Feature Engineering
- Used **CountVectorizer (Bag of Words)** to convert text into numerical features
- Combined text features with categorical features

### 3. Model Training
- Algorithm: **Random Forest Classifier**
- Train-test split: 80% training, 20% testing

### 4. Model Evaluation
- Metrics used:
  - Accuracy
  - Precision
  - Recall
  - F1-score
- Confusion Matrix visualization

### 5. Prediction
- Custom function implemented to predict sentiment for new reviews

## Results
- Achieved high accuracy on test data
- Model performs well in distinguishing positive and negative sentiments
- Important features include sentiment-heavy words like:
  - "love", "great", "excellent", "bad"

## How to Run the Project

### Step 1: Clone the Repository
```bash
git clone https://github.com/kadiwala1234/Customer-Review-Sentiment-Analysis.git
cd Customer-Review-Sentiment-Analysis
