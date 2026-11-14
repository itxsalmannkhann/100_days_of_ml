# TMDB Top 10,000 Movies Dataset

A movie dataset containing 10,000 records collected using the **The Movie Database (TMDB) API**. This dataset is designed for students, beginners, and data enthusiasts who want to practice Python, Pandas, data analysis, visualization, and machine learning.

## About the Dataset

This dataset contains information about 10,000 movies selected using TMDB's Top Rated Movies endpoint.

It can be used for:
- Exploratory Data Analysis (EDA)
- Data cleaning and preprocessing
- Data visualization
- Movie rating analysis
- Popularity analysis
- Beginner-friendly machine learning projects
- Natural Language Processing (NLP) experiments

**Dataset details:**

| Property | Description |
|---|---|
| Dataset Name | TMDB Top 10,000 Movies Dataset |
| Total Records | 10,000 movies |
| Data Format | CSV |
| Data Source | TMDB API |
| Main Language | Python |
| Primary Libraries | Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn |

## Dataset Structure

The dataset includes the following columns:

| Column | Description |
|---|---|
| `id` | Unique TMDB movie ID |
| `title` | Movie title |
| `overview` | Short description of the movie |
| `original_language` | Original language of the movie |
| `release_date` | Movie release date |
| `genre_ids` | List of TMDB genre IDs |
| `popularity` | TMDB popularity score |
| `vote_average` | Average user rating |
| `vote_count` | Total number of votes |

**Note:** If your CSV also contains `release_year` and `release_month`, these are derived from `release_date`.

## Possible Projects

You can use this dataset to build several data science projects.

### 1. Pandas Practice
- Load and explore the dataset.
- Select specific columns and rows.
- Filter movies based on ratings.
- Sort movies by popularity.
- Group movies by language.
- Find missing and duplicate values.
- Calculate average ratings and other statistics.

### 2. Data Visualization
- Distribution of movie ratings.
- Top 10 most popular movies.
- Number of movies released each year.
- Relationship between popularity and ratings.
- Average ratings by original language.
- Correlation between numerical features.

### 3. Machine Learning
- Predict movie ratings using available numerical and categorical features.
- Explore relationships between movie popularity and ratings.
- Build a basic recommendation system.
- Experiment with NLP using movie overviews.
- Perform clustering to identify groups of similar movies.

**Important:** A rating prediction model using popularity and vote count is primarily an educational exercise. These values may change over time and may not be available before a movie is released.

## Recommended Tools and Libraries

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## How to Use

1. Download the `movies.csv` file.
2. Open Jupyter Notebook, Google Colab, or VS Code.
3. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

4. Load the dataset:

```python
import pandas as pd

df = pd.read_csv("movies.csv")

print(df.head())
print(df.shape)
print(df.info())
```

5. Start exploring, analyzing, and visualizing the data.

## Data Source and Attribution

This dataset was collected using the **TMDB API**.

The Movie Database (TMDB): https://www.themoviedb.org/

API Documentation: https://developer.themoviedb.org/docs

Attribution notice:

"This product uses the TMDB API but is not endorsed or certified by TMDB."

This is an independent educational project and is not affiliated with or endorsed by TMDB.

**Data redistribution:** Please check TMDB's current Terms of Use and confirm that public redistribution of this compiled dataset is permitted before downloading or redistributing it.

## Important Notes and Limitations

- Movie ratings and popularity scores can change over time.
- Some records may contain missing information.
- Genre IDs are numeric identifiers and can be mapped to genre names using TMDB's genre list.
- This dataset represents a selected collection of movies, not the complete TMDB movie database.
- Since the movies were selected using a top-rated endpoint, the dataset may have selection bias.
- This dataset is intended for educational and practice purposes.

## Creator

**Created and maintained by Salman Khan**

I am a Computer Science (Artificial Intelligence) student interested in Artificial Intelligence, Machine Learning, Deep Learning, Data Science, and Software Development.

I created this dataset project to support practical learning and provide a resource for students and beginners exploring data analysis and machine learning.

**Connect with me:**

- **GitHub:** https://github.com/itxsalmannkhann
- **LinkedIn:** [Add your LinkedIn profile URL]
- **Email:** khanhackersalman@gmail.com

If you find this dataset useful, consider giving the repository or dataset an upvote and sharing it with other learners.

---

**Made with Python and curiosity by Salman Khan.**