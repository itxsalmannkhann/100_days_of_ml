# Open Library Books Dataset (6K+ Books)

## About the Dataset

The **Open Library Books Dataset** is a collection of book metadata sourced from the [Open Library](https://openlibrary.org/) public catalog.

This dataset was created as a beginner-friendly data collection and analysis project using Python and the Open Library Search API.

It provides structured book information that can be used for data analysis, exploratory data analysis (EDA), data visualization, and beginner-level machine learning experiments.

## Dataset Information

- **Source:** Open Library
- **Target Size:** Up to 6,000 plus book records
- **Format:** CSV
- **File Name:** `books-dataset.csv`
- **Data Type:** Structured tabular data

## Dataset Columns

| Column | Description |
|---|---|
| `openlibrary_key` | Unique Open Library Work identifier |
| `book_title` | Title of the book |
| `author` | Author name or names |
| `publication_year` | First known publication year of the work |
| `publisher` | Publisher information available in the catalog |
| `edition_count` | Number of editions associated with the work |

## Data Source

The data is obtained from Open Library, an open and publicly accessible book catalog maintained by the Internet Archive.

- Website: https://openlibrary.org/
- Search API: https://openlibrary.org/dev/docs/api/search
- API Endpoint: https://openlibrary.org/search.json
- Developer Documentation: https://openlibrary.org/developers

## Data Collection and Preparation

The dataset collection and preparation process uses:

1. Python for data collection.
2. Requests for API communication.
3. JSON parsing for extracting book metadata.
4. Pandas for data cleaning and transformation.
5. CSV export for dataset storage.

The preparation process includes handling missing values, removing duplicate work identifiers, and cleaning empty book titles.

## Potential Use Cases

This dataset can be used for:

- Exploratory Data Analysis (EDA)
- Identifying books with the most editions
- Exploring publication trends over time
- Analyzing author representation
- Studying publisher distribution
- Creating book recommendation experiments
- Practicing Python and Pandas
- Building beginner-level machine learning projects

## Python Usage

```python
import pandas as pd

# Load dataset
df = pd.read_csv("books_dataset.csv")

# Display first five records
print(df.head())

# Dataset information
print(df.info())

# Statistical summary
print(df.describe(include="all"))

# Top authors
print(df["author"].value_counts().head(10))

# Books with the most editions
print(
    df.sort_values(
        by="edition_count",
        ascending=False
    ).head(10)
)
```

## Data Limitations

- Some books may have missing author, publisher, or publication-year information.
- Publisher information may represent indexed edition metadata rather than every publisher associated with a work.
- Edition counts represent associated editions, not necessarily distinct physical copies.
- The dataset reflects the information available in Open Library at the time of collection.
- Catalog records may contain inconsistencies or incomplete metadata.

## Attribution and Data Source Citation

This dataset is derived from Open Library's public catalog.

**Please acknowledge the original data source when using or redistributing this dataset.**

Open Library:
https://openlibrary.org/

Open Library Search API Documentation:
https://openlibrary.org/dev/docs/api/search

Open Library Developer Center:
https://openlibrary.org/developers

Open Library Data Dumps:
https://openlibrary.org/developers/dumps

The original catalog records are maintained by Open Library and its contributors. This dataset is an independently prepared educational compilation and is not an official Open Library dataset release.

Please consult Open Library's current usage guidelines and licensing information before redistribution or commercial use.

## Developer / Creator

**Created by Salman Khan**

- GitHub: https://github.com/itxsalmannkhann
- LinkedIn: https://www.linkedin.com/in/itxsalmannkhann/ 
- Email: khanhackersalman@gmail.com

## Purpose

This project was created for educational purposes to practice API data collection, JSON processing, data cleaning, Python programming, and dataset preparation.

If you find this dataset useful, feel free to use it for learning, experimentation, and educational projects.

**Made with Python, Pandas, and Open Library.**

---

*Disclaimer: This dataset is not affiliated with, endorsed by, or officially maintained by Open Library or the Internet Archive.*