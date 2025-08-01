﻿#  Movie Recommendation System

A content-based movie recommendation system built using Python, leveraging natural language processing techniques and metadata from TMDB to suggest similar movies.

##  Datasets

- `tmdb_5000_movies.csv`: Contains metadata for 5000+ movies, including genres, overview, and keywords.
- `tmdb_5000_credits.csv`: Contains cast and crew information for the corresponding movies.

##  Features

- Merges movie and credit datasets based on the movie title.
- Extracts and processes key metadata: **genres**, **keywords**, **top cast members**, and **director**.
- Combines all relevant textual data into a single `tags` feature per movie.
- Applies NLP techniques to vectorize movie tags using `CountVectorizer`.
- Calculates cosine similarity between movie vectors.
- Provides top 5 similar movies as recommendations for a given title.

##  Tech Stack

- **Language**: Python 3.x  
- **Libraries**:
  - `pandas`, `numpy`: Data preprocessing and manipulation
  - `ast`: Safely parsing stringified Python literals
  - `scikit-learn`: Feature extraction (`CountVectorizer`) and similarity computation (`cosine_similarity`)
  - `pickle`: Model and data serialization


