AniFame: A Data-Driven Approach to Anime Success Prediction
🏆 Project Overview
Our project, AniFame, addresses a critical business challenge in the anime industry: the high cost of production versus the uncertainty of profitability. With an average 13-episode anime season costing around $2 million USD, many studios struggle to recoup their investment. The success of an anime, and a studio's profit margin is directly tied to its popularity. We developed a data-driven solution to help studios make informed decisions before production begins. By estimating an anime's potential 'mean' rating and predicting its 'success' probability, we provide actionable insights for optimizing projects to maximize profitability and ensure long-term viability.

<img width="1127" height="1266" alt="image" src="https://github.com/user-attachments/assets/2ac00474-d52c-4a5d-8440-fb5a816af9f7" />


🎯 Project Goals
The core objective of this project is to create a predictive model that empowers anime studios with strategic, data-backed decision-making capabilities. Our goals are:

Estimate Mean Rating: Predict the average rating an anime is likely to receive.

Predict Success Probability: Forecast the probability of an anime's commercial and critical success.

📊 Dataset & Methodology
We utilized the MyAnimeList (MAL) API to scrape a comprehensive dataset of anime produced from 2000 to 2021. This raw data was then processed through a robust data science pipeline.

The Data Science Pipeline
Data Collection:

Used the MAL API to recursively scrape thousands of anime data points from 2000 to 2021.

Data Cleaning & Preprocessing:

Handled missing values and removed irrelevant features.

Manipulated JSON data to extract key information.

Engineered new features, including a 'genres' time-series dataset.

Applied one-hot encoding to convert categorical data.

Exploratory Data Analysis (EDA) & Visualization:

Explored and visualized key relationships within the data, including:

Genre and studio trends over time.

The relationship between the 'mean' rating and variables like source material, media type, and audience demographics.

The correlation between 'mean' rating and viewership metrics.

Trends in episode count and duration.

Employed visualization techniques such as reducing data point size and opacity to effectively manage large datasets.

!(https://via.placeholder.com/800x400.png?text=Anime+Rating+vs+Genre+Visualization)

Regression Analysis:

Objective: To predict the 'mean' rating.

Models: Linear Regression, Lasso Regression, and Ridge Regression (Best).

Metrics: Explained Variance (R 
2
 ), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).

Classification Analysis:

Objective: To predict 'success' probability.

Models: LinearSVC, Decision Tree, and Random Forest (Best).

Metrics: Precision, Recall (TPR), F-score, out-of-bag (OOB) score, and ROC AUC score, with K-fold cross-validation to ensure model robustness.

💡 Key Insights & Recommendations
Our analysis has yielded actionable insights for anime studios:

Focus on Quality: Prioritize quality over quantity of production to maximize returns.

Seasonal Flexibility: Anime can be successful regardless of their broadcast season.

Source Material: Anime adapted from manga ('source_manga') have a strong correlation with success.

Media Type: 'media_type_movie' is a significant predictor of success, highlighting the potential of movie franchises.

Key Features: The most important features for predicting success are 'average_episode_duration', 'num_episodes', 'source_manga', 'media_type_movie', and 'rating_pg_13'.

🧠 What We Learned
This project was a comprehensive learning experience that touched on all aspects of the data science pipeline:

Data Collection: Gained hands-on experience scraping data using API calls.

Data Cleaning & Preprocessing: Mastered feature engineering, JSON manipulation, and generating time-series data.

EDA & Visualization: Developed effective visualization techniques for handling large datasets.

Machine Learning: Implemented and evaluated various regression and classification models, and gained a deep understanding of performance metrics.

🤝 Project Contributions
This project was a collaborative effort, with each team member bringing a unique skill set to the table:

Data Collection: Jing Qiang & Jing Hua

Data Cleaning & Preprocessing: Jing Qiang, Jing Hua & YinFeng

EDA & Visualization: Jing Qiang & Jing Hua

Regression: Jing Hua

Classification: Jing Qiang

Documentation & Presentation: Jing Qiang, Jing Hua & YinFeng

📚 References
MyAnimeList API Documentation

Anime News Network: Anime Production Costs

Medium: Data Analysis and Visualization on Anime

Towards Data Science: Linear Regression Models

BuiltIn: Random Forest Algorithm
