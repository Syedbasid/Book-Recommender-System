# 📚 Book Recommender System (Streamlit App)

## 🚀 Project Overview
This project is an **interactive Book Recommender System** built using **Python and Streamlit**.  
It recommends books to users using **Popularity Based** and **Collaborative Filtering** techniques.

The recommendation engine is trained using user book rating data and deployed as a web application using Streamlit.

---

## 🎯 Why Recommender Systems?
- Increase user engagement and satisfaction
- Reduce information overload
- Improve personalized content discovery

---

## 🧠 Recommendation Techniques Used

### 1️⃣ Popularity Based Recommendation
- Uses **average book ratings**
- Recommends **Top 50 most popular books**
- Same recommendations for all users
- Helpful for new users (cold start problem)

---

### 2️⃣ Collaborative Filtering (Book Based)
- Uses **user book interaction data**
- Each book is represented as a vector of user ratings
- Similarity between books is calculated using **Cosine Similarity**
- Recommends **Top 5 similar books** based on user selection

---

## 📐 Cosine Similarity Formula
\[
\cos(\theta) = \frac{A \cdot B}{|A||B|}
\]

Higher cosine value indicates higher similarity between books.

---

## 🧩 Project Files Explained

| File | Description |
|----|----|
| `app.py` | Streamlit web application |
| `Book_Recommendation.ipynb` | Data analysis, model building & similarity computation |
| `books.pkl` | Books metadata |
| `popular.pkl` | Precomputed Top 50 popular books |
| `pt.pkl` | Pivot table (user–book rating matrix) |
| `similarity_scores.pkl` | Cosine similarity scores between books |

---

## 🖥 Features of the Streamlit App
- 📊 Displays **Top 50 Popular Books**
- 🔍 Recommends **Top 5 similar books**
- ⚡ Fast response using precomputed similarity scores
- 🎨 Simple and user friendly interface

---

## 📷 App Screenshots
(Add screenshots inside the `screenshots/` folder)

---

## 🛠 Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- Streamlit

---

## ▶ How to Run the App Locally

```bash
pip install -r requirements.txt
streamlit run app.py
