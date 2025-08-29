# book-recommender-challenge
A K-Nearest Neighbors book recommendation engine using the Book-Crossings dataset
# Book Recommendation Engine with KNN

A collaborative filtering system built with `scikit-learn` and the Book-Crossings dataset.

## 🎯 Goal
Create a function `get_recommends(book_title)` that returns 5 similar books using **K-Nearest Neighbors**.

## 📊 Dataset
- 1.1M ratings from 90K users on 270K books
- Filtered to users with ≥200 ratings and books with ≥100 ratings
- Used cosine similarity on user-rating vectors

## 🚀 How It Works
1. Merge and filter data
2. Build user-book matrix
3. Train KNN on transposed matrix (books as vectors)
4. Return top 5 similar books

## 🧪 Example
```python
get_recommends("Where the Heart Is (Oprah's Book Club (Paperback))")
