# Hybrid Movie Recommender System (CF + CB)

This project implements a **hybrid movie recommendation system** using the [MovieLens Latest Small Dataset](https://grouplens.org/datasets/movielens/latest/).
It combines **Collaborative Filtering (CF)** based on user ratings and **Content-Based Filtering (CB)** based on movie genres.
The final hybrid model integrates both approaches to provide more robust recommendations.

---

## Notebook contents

The main notebook [`recommender.ipynb`](notebooks/recommender.ipynb) is structured as follows:

1. **Exploration** – initial analysis of the dataset.
2. **General classification** – most rated movies overview.
3. **Collaborative Filtering (CF)** – item-based cosine similarity on ratings.
4. **Content-Based Filtering (CB)** – similarity based on genres.
5. **Hybrid approach** – weighted combination of CF and CB.
6. **Evaluation** – metrics with *Precision@K*.
7. **Usage** – how to run the recommender functions.
8. **Examples** – user-based and item-based recommendation cases.
9. **Data export for Tableau** – generating CSVs for interactive dashboards.
10. **Acknowledgments** – credits to the MovieLens dataset and authors.

Exported versions for quick reading are available in the `reports/` folder:

* HTML (interactive in browser)
* PDF (static, for offline reading/sharing)

---

## Repository structure

```
.
├── data/          # Place MovieLens dataset here (not tracked in Git)
│   └── README.md
├── notebooks/
│   └── recommender.ipynb
├── reports/
│   ├── recommender.html
│   └── recommender.pdf
├── exports/       # CSV files for Tableau dashboards
├── requirements.txt
└── README.md
```

---

## How to run

1. Clone this repository:

   ```bash
   git clone https://github.com/<your-username>/movie-recommender-movielens.git
   cd movie-recommender-movielens
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset:

   * Get `ml-latest-small.zip` from [GroupLens](https://grouplens.org/datasets/movielens/latest/).
   * Unzip its contents inside the `data/` folder.

4. Open the notebook:

   ```bash
   jupyter notebook notebooks/recommender.ipynb
   ```

> ⚠️ Make sure the `data/` folder is in the same directory as the notebook.

---

## Tableau Dashboard

Interactive dashboards built with Tableau Public are based on the exported CSVs in `exports/`.

🔗 **Link to dashboard:** *(to be added once published)*

---

## Roadmap / Next Steps

* [ ] **Hyperparameter optimization**

  * Tune *k* for shrinkage
  * Tune *alpha* for hybrid weighting
  * Adjust relevance threshold for evaluation
* [ ] **Matrix Factorization**

  * Build a recommender using SVD
  * Compare results against current similarity-based methods

---

## Acknowledgments

This project uses the [MovieLens Latest Small Dataset](https://grouplens.org/datasets/movielens/latest/),
provided by [GroupLens Research](https://grouplens.org/) at the University of Minnesota.

Citation:

> Harper, F. Maxwell and Konstan, Joseph A. (2015).
> *The MovieLens Datasets: History and Context*.
> ACM Transactions on Interactive Intelligent Systems (TiiS) 5, 4, Article 19.
