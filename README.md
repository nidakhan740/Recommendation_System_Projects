
### Movie Recommendation System

This project builds a **Content-Based Movie Recommender System** using movie metadata such as genres, overview, keywords, and cast information. The goal is to suggest movies similar to a given title based on their content.

#### Problem Statement

Movie recommendation engines helps a user to find movies they might enjoy, based on their recently watched movie. This project suggests similar movies using features like genre, crew, and cast.

####  Dataset

- Source: [Kaggle - TMDB Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)
- Files used: `movies.csv`, `credits.csv`
- Key fields: `title`, `overview`, `genres`, `cast`, `crew`

#### Tools & Libraries

- Python
- Pandas, NumPy
- Scikit-learn (for cosine similarity)
- Ast (to parse stringified JSON columns)

####  Methodology

1. Merge movie and credit metadata
2. Clean and combine features like genres, cast, and keywords
3. Create a similarity matrix using combined feature vectors
4. Recommend top 5 movies most similar to the input movie

####  Sample Output

If you input `Avatar`, the system might recommend:
- John Carter  
- Guardians of the Galaxy  
- Star Trek  
- The Avengers  
- Star Wars

####  How to Use

1. Load the Jupyter notebook `Recommendation_System.ipynb`
2. Run all cells
3. Call the function:
```python
recommend("Iron Man")
```
4. It will print 5 similar movies


Author: Nida Khan

