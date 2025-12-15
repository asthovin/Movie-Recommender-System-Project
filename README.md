Movie Recommender System

This project is a content based movie recommendation system developed using Python. It recommends movies similar to a given movie by analyzing movie metadata and computing similarity between movies.

Dataset

The dataset used in this project is the TMDB Movie Metadata dataset.

Dataset name: TMDB Movie Metadata
Source: Kaggle
Link: https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata

This dataset contains information such as movie titles, genres, overviews, keywords, cast, crew, and other related metadata required to build a recommendation system.

Project Overview

The recommendation system is based on content filtering. It suggests movies by comparing their content features rather than using user ratings or behavior. The similarity between movies is calculated using textual data from multiple metadata fields.

Features Used

The following features from the dataset are used to generate recommendations:

Title
Overview
Genres
Keywords
Cast
Crew

These features are combined into a single text representation for each movie.

Working Methodology

First, the TMDB dataset is loaded and cleaned.
Relevant features are selected and merged into a single column.
Text data is vectorized using techniques such as Count Vectorizer or TF-IDF.
Cosine similarity is calculated between movie vectors.
Movies with the highest similarity scores are recommended.

Requirements

Python
Pandas
NumPy
Scikit-learn
NLTK

Example Usage

A movie title is given as input to the system.
The system returns a list of movies that are most similar to the input movie based on content similarity.

Limitations

This system is purely content based and does not use user ratings or collaborative filtering.
Scalability and performance optimization have not been implemented.

Conclusion

This project demonstrates the fundamental concepts of content based recommendation systems and provides a strong foundation for further enhancements such as collaborative filtering, hybrid models, or deployment as a web application.
