# Book Recommendation System

This project is a **Content-Based Book Recommendation System** built using Python. It recommends books similar to the one entered by the user based on user ratings and cosine similarity. The project is implemented in a Jupyter Notebook and uses machine learning concepts to generate meaningful and personalized book suggestions.

---

## Live Demo

- You can try the live app here:  
- [Book Recommendation System on Render](https://book-recommendation-system-9b57.onrender.com)
- *Please wait 20–30 seconds for the app to load — this delay is due to the Render free-tier service waking up the server.*

---

## Project Overview

The Book Recommendation System uses collaborative filtering and content-based filtering techniques to recommend books that are most similar to a user's input. The system works by:

- Creating a user-book rating matrix (pivot table)
- Computing cosine similarity scores between books
- Fetching top N books similar to the selected one

The final output is a list of 5 books along with their title, author name, and image.

---

## Problem Statement

With thousands of books available, users often struggle to choose what to read next. This project aims to solve this problem by building a system that recommends similar books based on reading preferences.

---

## Technologies Used

- Python
- Pandas
- NumPy
- scikit-learn
- Pickle
- Jupyter Notebook

---

## Dataset

The dataset used includes:
- `Books.csv` – Contains book details such as title, author, image URL, etc.
- `Ratings.csv` – Contains user ratings for books
- `Users.csv` – Contains information about the users

These datasets are merged and cleaned before model development.

---

## How the Model Works

1. **Data Cleaning & Preprocessing**:
   - Merged the books, users, and ratings datasets
   - Removed duplicate or irrelevant entries
   - Filtered books with few ratings to ensure quality recommendations

2. **Creating the Pivot Table**:
   - Constructed a matrix with users as rows and book titles as columns
   - Filled it with user ratings

3. **Calculating Similarities**:
   - Used cosine similarity from `sklearn` to calculate similarity between book vectors
   - Generated a similarity score matrix

4. **Making Recommendations**:
   - Created a function that takes a book title as input
   - Retrieves top 5 similar books using the similarity matrix
   - Displays recommended book titles, authors, and image links

---

## How to Run the Project

### 1. Clone the Repository
```bash
git clone https://github.com/HemaGarima/Book-Recommendation-System.git
cd Book-Recommendation-System
```
### 2. Install Required Libraries
```bash
pip install pandas numpy scikit-learn
```
### 3. Run the Jupyter Notebook
```bash
jupyter notebook book_recommendation_model.ipynb
```

## 4. Run the app
``` bash
python app.py
```
