# hybrid-movie-recommendation-system
A hybrid movie recommendation system using content-based and collaborative filtering with cosine similarity on the MovieLens dataset.
# Hybrid Movie Recommendation System

## Overview

This project implements a **Hybrid Movie Recommendation System** that suggests movies based on both:

* Content similarity (genres)
* User preferences (ratings)

It combines **Content-Based Filtering** and **Collaborative Filtering** to provide more accurate and personalized recommendations.

---

## Features

* Content-based filtering using **TF-IDF + Cosine Similarity**
* Collaborative filtering using **user similarity**
* Hybrid recommendation system combining both approaches
* Built using real-world **MovieLens dataset**
* Simple user input interface

---

## How It Works

### 1. Content-Based Filtering

* Uses movie **genres**
* Converts text into numerical vectors using **TF-IDF**
* Finds similarity using **cosine similarity**

### 2. Collaborative Filtering

* Uses **user ratings**
* Identifies users with similar preferences
* Recommends movies liked by similar users

### 3. Hybrid Model

* Combines both approaches to generate final recommendations

---

## Dataset

* Dataset: MovieLens (ml-latest-small)
* Files used:

  * `movies.csv`
  * `ratings.csv`

---

## Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn

---

## How to Run

1. Upload dataset files (`movies.csv`, `ratings.csv`)
2. Run the notebook / script
3. Enter:

   * Movie name
   * User ID

Example:

```python
movie_name = input("Enter movie name: ")
user_id = int(input("Enter user id (1–610): "))

print(hybrid_recommend(movie_name, user_id))
```

---

## Example Output

```
Enter movie name: Toy Story (1995)
Enter user id: 1

Recommended Movies:
1. Toy Story 2 (1999)
2. A Bug's Life (1998)
3. Finding Nemo (2003)
...
```

---

## Future Improvements

* Add Streamlit UI for better user experience
* Include movie descriptions for NLP-based recommendations
* Filter out already watched movies
* Deploy as a web application

---

## Learning Outcomes

* Understanding recommendation systems
* Implementing TF-IDF and cosine similarity
* Working with real-world datasets
* Building hybrid ML models

---

## Author

Sai Preeti Balaji
