# The Influence of Property Type on Booking Rates

This was our preliminary project exam, exploring how different Airbnb property types affect booking rates using data manipulation, exploratory analysis, and machine learning.

---

## Steps Overview

| Step                                             | Description                                                                                                                                                                                        |
| ------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Data Import and Exploration**                  | We loaded `listings.csv` into a PySpark DataFrame and previewed the first few rows to verify the dataset’s structure.                                                                              |
| **Identifying Data and Attributes**              | We examined each column’s name and data type to understand which fields were available.                |
| **Determining Data Types**                       | We classified columns as numerical, categorical, or mixed-type to decide how to preprocess them later.                                                                                             |
| **Data Quality and Assessment**                  | We checked for missing values and duplicates, then converted key fields (`bathrooms`, `price`, `host_response_rate`, `host_acceptance_rate`) to numeric.                                           |
| **Impute Missing Values**                        | We filled numerical columns with their median and categorical columns with their mode, and flagged mixed-type columns for special handling.                                                        |
| **Additional Wrangling & Feature Engineering**   | We discretized `price`, `accommodates`, and `review_scores_rating`; capped outliers; and created new features like `host_age`, `is_superhost`, and `total_availability`.                           |
| **Quantitative Statistics & EDA**                | We computed `booking_rate`, applied square root and log transformations to skewed fields, and generated visualizations for price, ratings, and geospatial booking patterns.                                  |
| **Application of Proximity (Distance Analysis)** | We calculated Euclidean distances on numeric features and visualized a sample distance matrix.  |
| **Machine Learning**                             | We created `booking_rate_category`, used Apriori to find association rules, and trained classification (Logistic Regression, Gaussian Naïve Bayes) and regression (SVR, Gradient Boosting) models. |

---

## Purpose  
Our project aimed to explore how different Airbnb property types influence booking rates by going through a full big data and machine learning pipeline. We worked with PySpark and Pandas to clean and transform a large dataset, dug into patterns using visual and geospatial analysis, and applied distance measures and Apriori to find deeper insights. We also built models to predict booking behavior by category and exact values. Along the way, we got to practice real-world data handling, sharpen our machine learning skills, and work together as a team to make sense of the results and explain them clearly.
