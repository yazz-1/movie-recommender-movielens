# Exports

This folder contains CSV files generated from the notebook, intended for interactive visualization in **Tableau Public** (or other BI tools).

Each file provides a summary or transformation of the MovieLens dataset and recommendation results.

## Files

* **`ratings_distribution.csv`**
  Histogram of ratings (from 0.5 to 5.0).

* **`movie_votes.csv`**
  Number of ratings per movie, including movie titles.

* **`avg_rating_per_genre.csv`**
  Average rating per genre, with genres expanded into separate rows.

* **`top_movie_similarities.csv`**
  Top-N most similar movies for each title based on the hybrid similarity model.

* **`user_activity.csv`**
  Number of ratings per user (user activity level).

* **`model_performance.csv`**
  Evaluation metrics (Precision@K) for Collaborative Filtering, Content-Based, and Hybrid models.

## Notes

* All files are generated automatically from the notebook in the `## Exportación de datos para Tableau` section.
* Files are lightweight summaries, not raw data.
* The original MovieLens dataset is not included here; see the `data/` folder for instructions.
