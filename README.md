# Investigate a Dataset: TMDb Movie Dataset Analysis

This project involves an exploratory data analysis (EDA) of the **TMDb Movie Dataset**. The dataset includes information about movies, including attributes such as ratings, popularity, genres, and financial data.

## Project Overview

The goal of this analysis was to:
1. Clean and preprocess the dataset.
2. Explore trends, distributions, and relationships within the data.
3. Answer specific research questions using visualizations and statistics.

## Research Questions

1. What are the most popular genres, and how do they correlate with revenue and ratings?
2. How does budget affect revenue and popularity?
3. How have movie runtimes and ratings evolved over the years?

## Data Cleaning

### Steps:
1. Dropped columns with excessive missing values (`homepage` and `tagline`).
2. Replaced missing values in `genres` and `keywords` columns with empty strings.
3. Parsed `genres` and `keywords` into lists for easier analysis.
4. Converted `release_date` to a proper datetime format for temporal analyses.

## Key Findings

### 1. Popularity and Ratings
- Most movies have a popularity score below 10, but a few outliers exceed 100.
- Action and Adventure genres are the most common and generally have higher popularity scores.

### 2. Budget and Revenue
- Revenue tends to increase with budget, but there are exceptions where low-budget movies achieve high revenue (e.g., Paranormal Activity).
- Most profitable genres include Action, Adventure, and Animation.

### 3. Trends Over Time
- Average movie runtime has remained steady, while movie budgets and revenues have increased since the 1980s.
- Movie popularity has seen a rise in recent years due to increased access to streaming platforms.

## Visualizations

### Popularity Distribution
![Popularity Distribution](images/popularity_distribution.png)

### Budget vs. Revenue
![Budget vs. Revenue](images/budget_vs_revenue.png)

### Average Revenue Over Time
![Average Revenue Over Time](images/average_revenue_over_time.png)

## How to Use This Repository

1. **View the Jupyter Notebook:** The analysis and visualizations are documented in the `Investigate_a_Dataset.ipynb` notebook.
2. **Dataset:** The dataset used is TMDb's movie dataset (provided separately).

## Dependencies

- Python 3.7+
- pandas
- matplotlib
- seaborn

Install the dependencies using:
```bash
pip install pandas matplotlib seaborn
