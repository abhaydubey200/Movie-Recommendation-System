# 🎬 Movie Recommendation System

A content-based Movie Recommendation System that suggests similar movies based on the metadata of a selected movie. The system uses machine learning and natural language processing techniques to recommend movies based on features like genre, overview, cast, crew, and keywords.

---

## 📌 Project Overview

This project demonstrates how to build a real-world recommendation engine using the TMDB 5000 Movie Dataset. Users can input the name of a movie, and the system recommends the top 5 most similar movies.

---

## ✅ Features

* Input any movie title from the dataset.
* Returns top 5 similar movies based on content features.
* Uses TF-IDF and cosine similarity for recommendation logic.
* Interactive input field using Jupyter Notebook widgets.
* Cleanly structured and well-documented.
* Easily extendable to include posters, ratings, and streaming links.

---

## 📊 Dataset

This project uses the **TMDB 5000 Movie Dataset**, which includes:

* Movie metadata (genres, overviews, keywords)
* Cast and crew information

**Files used:**

* `tmdb_5000_movies.csv`
* `tmdb_5000_credits.csv`

Available on [Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* scikit-learn
* ipywidgets
* Jupyter Notebook

---

## 📂 Project Structure

* **Data Loading & Merging**: Merges movie and credit data based on titles.
* **Data Cleaning**: Extracts relevant metadata like genres, keywords, cast, and crew.
* **Feature Engineering**: Combines important metadata into a single text feature (`tags`).
* **Vectorization**: Applies TF-IDF vectorizer to convert text into numerical data.
* **Similarity Matrix**: Computes cosine similarity between movie vectors.
* **Recommendation Engine**: Fetches top 5 movies most similar to the input.
* **Input Interface**: Accepts user input via an interactive text field.

---

## 🎯 Use Case

Users who enjoyed a specific movie can receive five more movie suggestions that share similar themes, genres, or other content characteristics.

---

## 🧠 How It Works (Conceptually)

1. Extract and clean metadata from both movie and credits dataset.
2. Combine selected metadata fields (overview, genres, cast, etc.) into one "tag".
3. Transform this tag column into numerical features using TF-IDF.
4. Measure similarity between all movies using cosine similarity.
5. Recommend the top 5 movies with the highest similarity scores to the input movie.

---

## 🚀 Future Improvements

* Add movie posters and metadata from TMDB API.
* Include filters for genre, release year, or rating.
* Add fuzzy search or auto-suggestions for input.
* Convert the project into a full-stack web application using Streamlit or Flask.
* Deploy the app on cloud platforms like Hugging Face, Render, or Heroku.

---

## 👨‍💻 Author

**Abhay Dubey**
🧑‍💻 MERN Stack | 📊 Data Analyst 
📧 [dubeyabhay430@gmail.com](mailto:dubeyabhay430@gmail.com)
🔗 [LinkedIn](https://linkedin.com/in/your-profile) | [GitHub](https://github.com/abhaydubey200)
