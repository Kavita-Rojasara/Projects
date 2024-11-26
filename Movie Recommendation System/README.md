# Movie Recommendation System Using Python

## Overview
This project implements a **Movie Recommendation System** using machine learning techniques. By leveraging content-based filtering, the system recommends movies based on their similarity to a given movie. It uses metadata such as genres, keywords, cast, and crew to compute similarities between movies.

## Features
- **Content-Based Filtering :**
  - Recommends movies similar to a selected movie based on their metadata.
- **Metadata Extraction :**
  - Combines information from genres, keywords, cast, and crew for personalized recommendations.
- **Cosine Similarity :**
  - Measures the similarity between movies to provide the best matches.
- **Efficient Preprocessing :**
  - Includes stemming and removal of spaces to standardize metadata.

## Workflow
1. **Data Loading :**
   - Loaded two datasets: `credits.csv` and `movies.csv`, containing metadata about movies.
2. **Data Preprocessing :**
   - Cleaned and merged datasets to create a unified dataset.
   - Extracted relevant columns: `movie_id`, `title`, `overview`, `genres`, `keywords`, `cast`, and `crew`.
3. **Feature Engineering :**
   - Created a `tags` column by combining text from `overview`, `genres`, `keywords`, `cast`, and `crew`.
   - Applied stemming and converted all text to lowercase for uniformity.
4. **Vectorization :**
   - Used `CountVectorizer` to convert text data into numerical vectors.
5. **Similarity Calculation :**
   - Computed **cosine similarity** between movies based on their feature vectors.
6. **Recommendation Function :**
   - Defined a function to recommend the top 5 similar movies for a given movie title.

## Technologies Used
- **Python :** Core programming language.
- **Pandas :** For data manipulation and cleaning.
- **NumPy :** For numerical operations.
- **Scikit-learn :** For vectorization and similarity computation.
- **NLTK :** For stemming.
- **CountVectorizer :** For converting text into feature vectors.

