# 🎓 Movie Recommendation System – A Research-Based Machine Learning Model

This project is a **content-based movie recommendation model** developed as part of a machine learning research effort. It explores how movie metadata (genres, overview, cast, crew, keywords) can be processed and analyzed using NLP and vector similarity techniques to provide intelligent recommendations.

---

## 🧠 Objective

The goal of this research-based model is to:

* Study the effectiveness of **content-based filtering** for recommendation systems.
* Use **vectorization (TF-IDF)** and **cosine similarity** to identify similar movies.
* Preprocess and engineer features from **unstructured movie metadata**.
* Build a scalable base model that can be extended into hybrid recommendation systems.

---

## 📊 Dataset Used

The model uses the **TMDB 5000 Movie Dataset**, which contains:

* Movie details: Title, overview, genres, keywords, popularity, etc.
* Cast and crew details: Actors, directors, etc.

**Files:**

* `tmdb_5000_movies.csv`
* `tmdb_5000_credits.csv`

**Source**: [Kaggle TMDB 5000 Movie Metadata](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

---

## 📂 Research Workflow

1. **Data Collection & Merging**

   * Merged `movies` and `credits` datasets on movie titles.

2. **Feature Extraction**

   * Extracted key fields: overview, genres, keywords, top 3 cast members, and director.

3. **Data Preprocessing**

   * Cleaned stringified JSON columns using Python’s `ast` module.
   * Concatenated all metadata into a single textual feature `tags`.

4. **Vectorization**

   * Applied `TfidfVectorizer` to convert `tags` into numerical vectors.

5. **Similarity Computation**

   * Used cosine similarity to compute pairwise similarity between movies.

6. **Recommendation Logic**

   * Given an input movie, retrieves the 5 most similar movies based on vector similarity.

---

## 🔍 Key ML & NLP Techniques Used

* **TF-IDF Vectorization**: For extracting feature importance from metadata.
* **Cosine Similarity**: For measuring closeness of movies in vector space.
* **Text Normalization**: Lowercasing, whitespace removal, and token merging.
* **Basic Feature Engineering**: Combining multiple metadata into one feature column.
* **Data Handling**: Robust JSON parsing and missing value handling.

---

## ✅ Research Outcome

* Successfully demonstrated that **content-based filtering** can effectively recommend movies using only metadata (no user data).
* Laid the foundation for future work on:

  * Hybrid recommender systems
  * Collaborative filtering
  * Real-time recommendation pipelines

---

## 🔬 Limitations

* Limited to movies present in the TMDB dataset.
* Recommendations may suffer from popularity bias (frequent terms dominate).
* No user-specific or feedback data used.

---

## 📌 Future Research Directions

* Integrate **poster similarity using image embeddings**.
* Add **collaborative filtering** (matrix factorization or deep learning).
* Implement **fuzzy matching or BERT embeddings** for better semantic understanding.
* Compare with **content-based filtering using neural embeddings (e.g., Doc2Vec, Sentence-BERT)**.
* Extend to **hybrid models** combining content + user behavior.

---

## 👨‍💻 Author

**Abhay Dubey**
🎓 Final Year B.Tech | 💻 ML Research Enthusiast | 🔧 MERN Stack Dev
📧 [dubeyabhay430@gmail.com](mailto:dubeyabhay430@gmail.com)
🔗 GitHub: [abhaydubey200](https://github.com/abhaydubey200)
