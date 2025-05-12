[🇺🇸 English](./README.md) | [🇰🇷 한국어](./README.ko.md)

# 📚 Book Recommender System

Welcome to **Team Bookaholic**'s project! This is a personalized book recommender system developed by Mason Liebe, Nami Kim, San Kim, and Wai-Sum Wu. Inspired by our learning from CIS5450 at the University of Pennsylvania, we built a recommender that goes beyond Amazon's generic "you might like" suggestions.

🔗 Try it out: [Streamlit App](https://cis545-book-project-60m9b4032y8.streamlit.app/Parameter_based_book_recommender)  
🖥️ Front-end repo: [https://github.com/wuwaisum0517/cis545-book-project](https://github.com/wuwaisum0517/cis545-book-project)


## Project Overview

We started with a real-world challenge:  
> *"What do I read next?"*

To answer that, we processed and analyzed a large dataset from BookCrossing, using machine learning models to predict which books a user will enjoy—based on their past ratings and demographics like age and location.


## Dataset

Sourced from Kaggle: [Book Recommendation Dataset](https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset)

- **Users:** `user_id`, `location`, `age`  
- **Books:** `ISBN`, `title`, `author`, `publisher`, `year`, `cover image URL`  
- **Ratings:** `user_id`, `ISBN`, `rating` (1–10 scale)

We picked this dataset because it includes demographic features, which helped us build **parameter-based recommenders** with more personalization.


## Features

- **Collaborative Filtering** based on user-book ratings matrix
- **Content-based Filtering** using user location and age
- **Cold-start handling** via clustering and metadata
- **Streamlit interface** to interact with different recommender modes


## To view the notebook 
https://github.com/namikimlab/book-recommender/blob/main/Final_notebook.ipynb


##  Tech Stack

| Category         | Tools / Libraries                          |
|------------------|---------------------------------------------|
| **Language**      | Python 3                                   |
| **Data Handling** | Pandas, NumPy                              |
| **Visualization** | Matplotlib, Seaborn                        |
| **Machine Learning** | Scikit-learn, KMeans                    |
| **App Framework** | Streamlit                                 |
| **Environment**   | Jupyter Notebook                           |
| **Data Source**   | BookCrossing Dataset from Kaggle           |


## Learnings & Challenges
This project helped us practice:  
Data cleaning and wrangling of large, noisy datasets  
Building ML models for sparse matrices  
Dealing with missing values, outliers, and cold-start problems  
Designing a simple, intuitive user interface  
We also had a lot of fun. 😄  


