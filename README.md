# NLP-Sentiment-Analysis

NLP sentiment analysis pipeline achieving 92% accuracy, deployed via Flask and Streamlit

# Amazon E-Commerce Sentiment Analysis & Deployment

An end-to-end NLP sentiment analysis pipeline achieving **92% accuracy**, deployed as a live web application via Flask and Streamlit.

## 📌 Project Overview
This project analyses Amazon e-commerce customer reviews to classify sentiment as positive, negative, or neutral. The final model was selected based on rigorous evaluation across five algorithms and deployed for real-time prediction.

## 🛠 Tools & Technologies
- **Language:** Python
- **NLP Libraries:** NLTK, VADER, TextBlob
- **ML Libraries:** Scikit-learn, Pandas, NumPy
- **Feature Engineering:** Bag of Words (BOW), TF-IDF
- **Deployment:** Flask (REST API), Streamlit (interactive front-end)
- **Environment:** Jupyter Notebook (development), VS Code (deployment)

## 📊 Methodology

### 1. Data Collection & Cleaning
- Collected large-scale customer review data from secondary sources
- Performed data quality checks — handling missing values, removing duplicates, and validating data types
- Identified and resolved gaps and inconsistencies before analysis

### 2. Feature Engineering
- Applied **Bag of Words (BOW)** vectorization
- Applied **TF-IDF** (Term Frequency-Inverse Document Frequency) vectorization
- Transformed raw text into structured, analysis-ready numerical features

### 3. Model Training & Evaluation
Five NLP classification models were trained and evaluated:

| Model | Approach |
|---|---|
| Logistic Regression | Linear classification |
| Naïve Bayes | Probabilistic classification |
| Support Vector Machine (SVM) | Margin-based classification |
| VADER | Rule-based sentiment analysis |
| TextBlob | Lexicon-based sentiment analysis |

### 4. Model Selection
The optimal model was selected based on **precision-recall analysis** — achieving **92% accuracy** on the review text-only approach (ratings excluded to avoid artificial signal from missing data).

### 5. Deployment
- **Flask** — REST API backend for real-time inference
- **Streamlit** — interactive front-end for user input and prediction display
- Both deployed via **VS Code** for production

## 📈 Results
- **Best accuracy:** 92%
- **Input:** Customer review text only
- **Output:** Sentiment classification (Positive / Negative / Neutral)

## 🗂 Repository Structure
```
├── Amazon_Sentiment_Analysis.ipynb    # Main Jupyter notebook
├── app.py                             # Flask API
├── streamlit_app.py                   # Streamlit front-end
├── model.pkl                          # Saved model
└── README.md                          # Project documentation
```

## 🚀 How to Run
1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run Flask: `python app.py`
4. Run Streamlit: `streamlit run streamlit_app.py`

## 👤 Author
**Maryann Anaebo**
- LinkedIn: [linkedin.com/in/obianuju-anaebo](https://linkedin.com/in/obianuju-anaebo)
- GitHub: [github.com/iammaryann](https://github.com/iammaryann)