# TMDB Movie Data Analysis
Egwd professional second project

This project focuses on analyzing a dataset containing information about 10,000 movies collected from The Movie Database (TMDB). The dataset includes various attributes such as user ratings, revenue, budget, genres, and more. The goal of this project is to gain insights and answer questions related to movie genres, popularity, and revenue.

## Dataset Information

The dataset consists of the following columns:

- `id`: Unique identifier for each movie
- `imdb_id`: IMDB identifier for each movie
- `popularity`: Popularity score of the movie
- `budget`: Budget of the movie
- `revenue`: Revenue generated by the movie
- `original_title`: Title of the movie
- `cast`: Cast members of the movie
- `director`: Director of the movie
- `tagline`: Tagline of the movie
- `keywords`: Keywords associated with the movie
- `overview`: Overview of the movie
- `runtime`: Duration of the movie in minutes
- `genres`: Genres of the movie
- `production_companies`: Production companies involved in the movie
- `release_date`: Release date of the movie
- `vote_count`: Number of votes received by the movie
- `vote_average`: Average rating of the movie
- `release_year`: Year of release
- `budget_adj`: Budget adjusted for inflation
- `revenue_adj`: Revenue adjusted for inflation

## Questions of Interest

The project aims to explore and answer the following questions:

1. Which genres are most popular from year to year?
2. What kinds of properties are associated with movies that have high revenues?

## Tools and Libraries Used

The analysis is performed using Python and various libraries:

- Pandas: For data manipulation and analysis
- NumPy: For numerical computations
- Matplotlib: For data visualization
- Seaborn: For enhanced data visualization

## Data Loading and Cleaning

The data is loaded from the "tmdb-movies.csv" file using the `Load_data()` function. The unnecessary columns such as `id`, `imdb_id`, `homepage`, `tagline`, `overview`, `keywords`, and `production_companies` are dropped from the dataset to focus on relevant attributes.

Missing data in the columns `cast`, `director`, and `genres` are removed from the dataset since the information in those rows is not complete or useful for the analysis.

## Exploratory Data Analysis

The data is explored using various statistical measures and visualizations. Descriptive statistics are calculated for attributes such as popularity, budget, revenue, runtime, vote count, and vote average. Histograms are plotted to visualize the distribution of the data.

## Research Question 1: Which genres are most popular from year to year?

To answer this question, the genres column is split into separate rows using the `split_genres()` function. This creates a new dataframe, `df_genres`, where each row corresponds to a single genre associated with a movie. The popularity of each genre is then analyzed over the years to identify the most popular genres.

## Research Question 2: What kinds of properties are associated with movies that have high revenues?

To address this question, the relationship between different properties and movie revenue is explored. Statistical measures, such as correlation coefficients, are calculated to determine the strength and direction of the relationship. Visualizations, such as scatter plots, are used to visualize the relationship between revenue and other attributes like budget, popularity, and vote average.

## Conclusion

This project provides insights into the TMDB movie dataset and addresses two key questions related to movie genres, popularity, and revenue. By analyzing the data and visualizing the relationships between various attributes, we can gain a better understanding of the factors that
