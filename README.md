# Netflix Content Analytics & Recommendation System

![Netflix](https://img.shields.io/badge/Netflix-E50914?style=for-the-badge&logo=netflix&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Power BI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit Learn](https://img.shields.io/badge/ScikitLearn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)

## 📌 Project Overview
End-to-end data analytics and machine learning project analyzing Netflix's content 
library of 8,800+ titles. Built a content-based recommendation engine using NLP 
techniques and visualized insights through an interactive Power BI dashboard.

## 🛠️ Tools & Technologies
- **Python** — Data cleaning, EDA, Machine Learning
- **Pandas & NumPy** — Data manipulation
- **Matplotlib & Seaborn** — Data visualization
- **Scikit-learn** — TF-IDF Vectorization, Cosine Similarity
- **WordCloud** — Text visualization
- **Power BI** — Interactive dashboard

## 📁 Dataset
- Source: [Netflix Movies and TV Shows - Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- 8,800+ titles with 12 features
- Features: title, type, director, cast, country, date_added, 
  release_year, rating, duration, listed_in, description

## 🔍 Project Phases

### Phase 1: Data Cleaning
- Handled 2,634 missing director values
- Filled 825 missing cast entries
- Standardized date formats
- Removed dirty/incorrect type values
- Feature engineering: extracted year_added, month_added, duration_value

### Phase 2: Exploratory Data Analysis
- Movies vs TV Shows distribution (69.6% vs 30.4%)
- Netflix content growth peaked in 2019-2020
- USA, India, UK are top content producing countries
- International Movies & Dramas are most common genres
- TV-MA is the most common content rating

### Phase 3: Recommendation Engine
- Combined title, director, cast, genre and description into content tags
- Applied TF-IDF Vectorization (5000 features)
- Calculated Cosine Similarity across all titles
- Function returns top N similar titles with similarity scores

### Phase 4: Power BI Dashboard
- 3-page interactive dashboard with Netflix red theme
- Page 1: Content Overview (KPIs, Pie chart, Line chart)
- Page 2: Genre & Country Analysis (Bar charts, Slicers)
- Page 3: Recommendation Results Table

## 🤖 How the Recommender Works
```python
# Example usage
get_recommendations('Stranger Things', n=10)

# Returns:
# Beyond Stranger Things  →  similarity: 0.553
# Equilibrium             →  similarity: 0.196
# Things Heard & Seen     →  similarity: 0.188
```
## 📊 Dashboard Screenshots

### Page 1 — Content Overview
![Page 1](dashboard_page1.png)

### Page 2 — Genre & Country Analysis
![Page 2](dashboard_page2.png)

### Page 3 — Recommendations
![Page 3](dashboard_page3.png)

## 📈 EDA Visualizations

### Movies vs TV Shows
![Pie](outputs/movies_vs_tvshows.png)

### Content Added Per Year
![Line](outputs/content_per_year.png)

### Top 10 Countries
![Countries](outputs/top_countries.png)

### Top 10 Genres
![Genres](outputs/top_genres.png)

### Word Cloud
![Wordcloud](outputs/wordcloud.png)

## 👩‍💻 Author
**Namrata Chaurasia**  
[GitHub](https://github.com/namratac05) | 
[Tableau](https://public.tableau.com/app/profile/namrata.chaurasia)
