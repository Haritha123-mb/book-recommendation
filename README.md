# 📚 Book Recommendation System – Book-Crossing Dataset

This project analyzes the **Book-Crossing dataset** and applies recommendation algorithms to suggest books to users.  
It involves **Exploratory Data Analysis (EDA)**, **data preprocessing**, and **collaborative filtering** techniques (both model-based and memory-based).

---

## 📊 Conclusion

- In EDA, the **Top-10 most rated books** were mainly **novels** (e.g., *The Lovely Bone*, *The Secret Life of Bees*).  
- Most readers were aged **20–35** and primarily from **USA, Canada, UK, Germany, and Spain**.  
- Ratings distribution showed **most books have high ratings**, with the majority rated **8**; ratings below 5 were rare.  
- Authors with the most books: **Agatha Christie, William Shakespeare, Stephen King**.  
- In modelling:
  - **Model-based Collaborative Filtering (CF)**: SVD performed better than NMF (lower Mean Absolute Error).  
  - **Memory-based Collaborative Filtering (CF)**: Item-item CF outperformed user-user CF (lower computation cost).  

---

## 📂 Book-Crossing Dataset Overview

The dataset consists of three main files:

1. **Users**
   - Contains anonymized `User-ID` (integer)
   - Demographics: `Location`, `Age` (may be NULL if missing)

2. **Books**
   - Each book has a valid ISBN
   - Information: `Book-Title`, `Book-Author` (only first author), `Year-Of-Publication`, `Publisher`
   - Cover image URLs from Amazon:
     - `Image-URL-S` (small)
     - `Image-URL-M` (medium)
     - `Image-URL-L` (large)

3. **Ratings**
   - Ratings linked to books and users
   - Scale: `1–10` (explicit rating, higher = better)
   - `0` means implicit rating (no explicit score)

---

## 🚀 Techniques Used

- **Exploratory Data Analysis (EDA)**: Understanding user demographics, book popularity, and rating trends.  
- **Data Preprocessing**: Handling missing values, cleaning text, and merging datasets.  
- **Recommendation Algorithms**:
  - Model-based CF: **SVD**, **NMF**
  - Memory-based CF: **User-User CF**, **Item-Item CF**

---

## 📌 Key Findings

- Younger readers (20–35) dominate the dataset.  
- The dataset is skewed towards popular novels and Western readers.  
- Item-item CF is computationally more efficient for large datasets.  

---

## 📜 License

This dataset is from the **[Book-Crossing Dataset](http://www2.informatik.uni-freiburg.de/~cziegler/BX/)** and is intended for **educational and research purposes**.
