# 🎬 AniFame: Predicting Anime Success with Data Science  

## 📌 Business Problem  
Producing anime is **extremely costly**, averaging **$2M for a 13-episode season** (Anime News Network, 2015). Yet, many projects fail to recoup this investment, leaving studios struggling for survival.  
The challenge: **How can studios predict whether an anime will be successful before production?**  

AniFame tackles this by predicting **mean ratings** and **success probability** using machine learning. This helps studios:  
- 🎯 Identify profitable projects early  
- 💡 Fine-tune anime concepts before release  
- 📈 Reduce financial risk and maximize ROI  

---

## 🎯 Project Goal  
To build a **data-driven framework** that forecasts anime success using historical data from **MyAnimeList (MAL)**.  
The project leverages **EDA + ML models** to answer:  
- Are ratings predictable based on features like studio, genre, and source?  
- Which factors most influence anime popularity and profitability?  
- What strategies should studios adopt to ensure long-term survival?  

---

## 📂 Dataset  
- Source: [MyAnimeList API](https://myanimelist.net/apiconfig/references/api/v2)  
- Timeframe: **2000–2021**  
- Scraped, cleaned, and processed into structured CSV files  
- Focus: *Movies* and *Ratings* datasets for prediction tasks  

---
<img width="1127" height="1266" alt="image" src="https://github.com/user-attachments/assets/b7fc9fce-218e-4e83-af50-853bfad09353" />


## 🔬 Methodology & Pipeline  

### 1️⃣ Data Collection  
- Recursive scraping of thousands of anime entries from MAL API  

### 2️⃣ Data Cleaning & Preprocessing  
- Removed irrelevant features & handled missing values  
- JSON conversion & manipulation  
- Engineered features: genre time-series, one-hot encoding  
- Exported cleaned datasets for ML  

### 3️⃣ Exploratory Data Analysis (EDA)  
- Trends in **genres**, **studios**, and **seasonality**  
- Relationship between **ratings, popularity, viewership fractions**  
- Analysis of **episode count** and **duration trends**  

### 4️⃣ Regression Models  
- Linear Regression, Lasso, Ridge (🏆 **Best**)  
- Metrics: R², MSE, RMSE  

### 5️⃣ Classification Models  
- LinearSVC, Decision Tree, Random Forest (🏆 **Best**)  
- Metrics: Confusion Matrix, Precision, Recall, F-score, ROC AUC  

---

## 📊 Key Insights & Recommendations  

### 📌 Findings  
- **Quality > Quantity**: More episodes ≠ higher success  
- **Seasonality doesn’t matter**: Animes perform consistently across seasons  
- **Fan-service ≠ profitability**: More positive views don’t guarantee financial returns  
- **Movies matter**: Anime movie franchises drive long-term profitability  

### ⭐ Key Features Driving Success  
- `average_episode_duration`  
- `num_episodes`  
- `source_manga`  
- `media_type_movie`  
- `rating_pg_13`  

---

## 💡 Business Impact  
AniFame provides **actionable insights** for anime studios:  
- 🎥 Focus budgets on **anime movies & manga-based adaptations**  
- 📊 Use **data-driven forecasting** before committing millions in production  
- 💰 Increase survival rates in a highly competitive, high-cost industry  

---

## 🧑‍💻 What I Learned  
- API scraping & large-scale data collection  
- JSON preprocessing & feature engineering  
- Handling large datasets with **EDA visualization techniques**  
- Model selection & evaluation with regression/classification metrics  



---

## 📚 References  
- [MAL API](https://myanimelist.net/apiconfig/references/api/v2)  
- [Anime Production Costs](https://www.animenewsnetwork.com/interest/2015-08-13/anime-insiders-share-how-much-producing-a-season-costs/.91536)  
- [Data Science Resources](https://towardsdatascience.com/linear-regression-models-4a3d14b8d368)  
- [Random Forest Guide](https://builtin.com/data-science/random-forest-algorithm)  
