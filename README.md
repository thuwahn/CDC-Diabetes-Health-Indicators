# **SVD-in-Movie-Recommendation-Systems**

## Description
This project implements a movie recommendation system using **Singular Value Decomposition (SVD)**. It features **a simple SVD** for baseline recommendations and **an advanced SVD** that integrates Collaborative Filtering, Content-Based Filtering, and a Hybrid Model to boost accuracy and tackle the cold-start problem for new users and movies.

## About Data 

#### **Diabetes Health Indicators Dataset**

The Diabetes Health Indicators dataset contains health-related survey responses from the CDC’s Behavioral Risk Factor Surveillance System (BRFSS), providing information on chronic diseases, lifestyle habits, and demographic factors in 2015. Key details include:

- **Scale:**
    - 25,000,095 ratings
    - 1,093,360 tags
    - 62,423 movies
    - 162,541 users

- **User Criteria:** Randomly selected users, each with at least 20 movie ratings. No demographic information is included, ensuring anonymity.

- **Data Files:** 6 CSV files:
    - **`ratings.csv`**: User movie ratings (`userId`, `movieId`, `rating`, `timestamp`)
    - **`tags.csv`**: User-applied movie tags (`userId`, `movieId`, `tag`, `timestamp`)
    - **`movies.csv`**: Movie details (`movieId`, `title`, `genres`)
    - **`links.csv`**: Links to external movie databases (IMDb, TMDb) (`movieId`, `imdbId`, `tmdbId`)
    - **`genome-scores.csv`**: Tag relevance scores for movies (`movieId`, `tagId`, `relevance`)
    - **`genome-tags.csv`**: Descriptions of tags in the tag genome (`tagId`, `tag`)

- **User and Movie IDs:**
    - User IDs are anonymized and consistent across `ratings.csv` and `tags.csv`.
    - Movie IDs are consistent across `ratings.csv`, `tags.csv`, `movies.csv`, and `links.csv`.

> **To download the data, you can access the `data` folder or download it from the following link: [here](https://grouplens.org/datasets/movielens/25m/)**

## Project Structure

| **Folder**              | **Description**                                              |
|-------------------------|--------------------------------------------------------------|
| diabetes.html                | Contains the MovieLens ml-25m dataset used for training and testing the models. |
| diabetes.pdf                  | Implements the simple SVD model for baseline movie recommendations. |


