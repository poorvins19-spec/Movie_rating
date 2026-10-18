# 🎬 Movie Market Analysis

## 📌 Project Overview

This project analyzes movie ratings and box-office revenue for **CineData Studios** using Python. The goal is to understand movie quality trends, compare genres, evaluate financial performance, and identify critically successful movies.

The analysis uses data analysis and visualization techniques to help support data-driven decisions about future movie productions.

## 🎯 Objectives

- Calculate the average IMDb rating across all movies.
- Compare average IMDb ratings across different genres.
- Identify the highest-rated genre.
- Calculate total box-office revenue for each genre.
- Visualize genre-wise revenue using a bar chart.
- Examine the distribution of IMDb ratings using a histogram.
- Classify movies as hits or non-hits based on their ratings.
- Calculate the total number and percentage of hit movies.

## 🛠️ Technologies Used

- **Python** — programming language
- **Pandas** — data manipulation and analysis
- **Matplotlib** — data visualization
- **Seaborn** — statistical charts and visualization
- **Jupyter Notebook / Google Colab** — interactive analysis environment

## 📂 Project Structure

```text
movie-market-analysis/
│
├── README.md
├── movie_rating.ipynb
└── movie_ratings_dataset.csv
```

**Note:** The CSV file must be added separately if it is available and you have permission to share it.

## 📊 Dataset Information

The notebook expects a dataset named `movie_ratings_dataset.csv`.

The following columns are referenced in the analysis:

| Column | Description |
|---|---|
| `Movie_ID` | Identifier for each movie |
| `Genre` | Genre associated with a movie |
| `IMDB_Rating` | IMDb rating of a movie |
| `Box_Office_Millions` | Box-office revenue, expressed in millions |

The dataset file was not included with the uploaded notebook, so its actual size, source, and record count have not been verified.

## 🔍 Analysis Performed

### 1. Average IMDb Rating

Calculates the mean of the `IMDB_Rating` column to establish an overall rating benchmark for the movies in the dataset.

### 2. Genre Rating Analysis

Groups movies by `Genre` and calculates the average IMDb rating for each genre. The genre with the highest average rating is identified.

### 3. Box-Office Revenue Analysis

Calculates the total box-office revenue for each genre and displays the results using a bar chart.

The chart includes a title, axis labels, rotated genre names, and formatting for readability.

### 4. IMDb Rating Distribution

Creates a histogram to show how movie ratings are distributed across the dataset. The notebook also displays descriptive statistics for the rating column.

### 5. Hit Movie Identification

Creates a new Boolean column named `Hit` using this rule:

- **Hit = True:** IMDb rating is greater than or equal to 8.0.
- **Hit = False:** IMDb rating is below 8.0.

### 6. Hit Movie Summary

Counts the movies classified as hits and calculates the percentage of hits in the dataset.

## ⚙️ Installation and Setup

Make sure Python is installed on your computer. Install the required libraries using:

```bash
pip install pandas matplotlib seaborn jupyter
```

## ▶️ How to Run the Project

### Option 1: Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload `movie_rating.ipynb`.
3. Upload `movie_ratings_dataset.csv` to the Colab session.
4. Run the notebook cells in order.

The notebook currently uses the Google Colab file path `/content/movie_ratings_dataset.csv`.

### Option 2: Run Locally

1. Download or clone this repository.
2. Install the required Python libraries.
3. Place `movie_ratings_dataset.csv` in the same folder as the notebook.
4. In the notebook, change the dataset-loading line to:

```python
df = pd.read_csv("movie_ratings_dataset.csv")
```

5. Open the notebook in Jupyter and run the cells in order.

## 📈 Expected Outcomes

After running the notebook, the analysis produces:

- The overall average IMDb rating.
- Average IMDb ratings by genre.
- The highest-rated genre.
- Total box-office revenue by genre and a bar chart.
- A histogram and descriptive statistics for IMDb ratings.
- Hit and non-hit movie counts.
- The percentage of movies classified as hits.

Actual numerical findings depend on the dataset used.

## 💡 Potential Applications

This analysis could help a media strategy team:

- Compare audience or critic rating patterns across genres.
- Explore which genres generate greater total box-office revenue.
- Identify movies that meet a chosen rating threshold.
- Support further investigation into movie production and investment decisions.

These results can support exploration, but they do not by themselves establish that a genre will be profitable in the future.

## 🚀 Future Improvements

- Analyze the relationship between IMDb ratings and box-office revenue.
- Compare revenue and average ratings in a combined dashboard.
- Add movie release years and trends over time, if available.
- Explore the impact of production budgets and marketing costs, if available.
- Add data cleaning, missing-value checks, and outlier analysis.
- Build an interactive dashboard using Plotly or Streamlit.

## 👩‍💻 Author

**Poorvi N S**

B.Tech — Artificial Intelligence and Machine Learning

## 📜 License

This project is intended for educational and portfolio purposes. Check the dataset's license and sharing permissions before redistributing it.
