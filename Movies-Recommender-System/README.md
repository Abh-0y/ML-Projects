# Movie Recommendation System

A **multi-approach Movie Recommendation System** that generates personalized movie suggestions using **Weighted Rating**, **Genre-Based**, **Content-Based**, **Collaborative Filtering**, and **Hybrid Recommendation** techniques.

---

## Project Objective

To design and compare multiple recommendation strategies and understand how different algorithms influence movie recommendations in real-world platforms.

---

## Recommendation Techniques Implemented

### Weighted Rating Recommendation
- Uses IMDb’s **weighted rating formula**
- Ranks movies based on:
  - Average rating
  - Number of votes
- Solves the bias of highly rated but low-vote movies

### Genre-Based Recommendation
- Recommends top movies within a selected genre
- Useful for users with clear genre preferences

### Content-Based Recommendation
- Analyzes movie metadata such as:
  - Overview
  - Genres
  - Keywords
  - Cast
- Uses **TF-IDF Vectorization** and **Cosine Similarity**
- Recommends movies similar in content

### Collaborative Filtering
- Recommends movies based on **user–item interactions**
- Identifies users with similar preferences
- Suggests movies liked by similar users

### Hybrid Recommendation System
- Combines **content-based** and **collaborative filtering**
- Improves recommendation accuracy
- Reduces limitations of individual methods

---

## Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- NLP (TF-IDF)
- Jupyter Notebook
