# 🎬 IMDB Ratings vs. Votes  
*Exploring the relationship between IMDB ratings and the number of votes for TV shows released since 1999.*  

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)  
![pandas](https://img.shields.io/badge/pandas-Data%20Analysis-green?logo=pandas)  
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)  

---

## 📌 Overview  
This project analyzes whether higher-rated TV shows also receive higher vote counts on IMDB. Using pandas, the dataset was cleaned, filtered, and grouped to evaluate average votes by rating categories. The analysis focuses specifically on TV shows from the year 1999 onward, often called the "Golden Age of Television."  

---

## 📊 Dataset  
- **Source:** Provided by TripleTen Bootcamp (`movies_and_shows.csv`).  
- **Size:** ~8,500 rows (movies and shows).  
- **Key Features:**  
  - `title` – title of the movie or show  
  - `release_year` – release year  
  - `imdb_score` – rating (1–10 scale)  
  - `imdb_votes` – number of votes  

- **Filtering Applied:**  
  - Restricted to TV shows released in **1999 or later**  
  - Grouped IMDB scores into integer buckets  
  - Excluded buckets with very low sample sizes  

---

## ⚙️ Methods & Tools  
- **Library Used:** pandas  
- **Techniques:**  
  - Data selection & filtering  
  - Grouping and aggregation  
  - Outlier exclusion  

---

## 📈 Results  
- Outlier groups (ratings 2, 3, and 10) were excluded due to insufficient data.  
- Ratings **7, 8, and 9** had the **highest average vote counts**, supporting the hypothesis that highly rated shows generate more audience engagement.  
- About **94% of the dataset remained** after filtering, giving high confidence in the findings.  

---

## 💡 Key Insights  
- Strong evidence that **critical acclaim (ratings 7–9) aligns with higher audience participation (votes)**.  
- Lower-rated shows generally drew fewer votes, with minor exceptions.  
- Analysis reinforces the connection between audience reception and overall popularity.  

---

## 🗂 Repo Structure  
```
imdb-rating-votes/
│
├── notebooks/ 
├── data/ 
├── requirements.txt 
├── LICENSE 
└── README.md
```
---

## 🚀 How to Run  
1. Clone the repo:  
   ```bash
   git clone https://github.com/Flamingo-Rocker/imdb-rating-votes.git
   cd imdb-rating-votes
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
3. Open the notebook in notebooks/

---

## 📦 Requirements
pandas==2.3.2

---

## 🙏 Acknowledgment
Developed as part of the TripleTen Data Science Bootcamp, demonstrating data cleaning, grouping, and exploratory data analysis using pandas.
