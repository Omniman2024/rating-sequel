#### rating-sequel
# Exploratory Data Analysis : possible effect on movie ratings with progressing sequels. 

This project analyzes the influence of sequels on IMDb ratings for movie series. Using a cleaned dataset of movies and their corresponding series orders and ratings, we explore trends, correlations, and visual patterns to understand how sequels perform compared to their predecessors.

---

##  Dataset

- **File:** `Movies - Cleaned.csv`

This dataset is available in Kaggle - https://www.kaggle.com/datasets/thedevastator/movies-with-sequels-imdb-analytics-and-ratings

---

##  Analysis Performed

###  Data Cleaning  
- Removed all series where **any movie had a missing IMDb rating** to ensure fair trend analysis.

###  Series Grouping  
- Grouped series based on number of movies:
  - **2-movie series**
  - **3-movie series**
  - **4-movie series**
  - **5-movie series**

###  Correlation Analysis  
- Calculated **Pearson correlation coefficient** between `Order` and `IMDb Rating` within each group to see if ratings decline with sequels.
- Results:
  - 2-movie series: `-0.36`
  - 3-movie series: `-0.34`
  - 4-movie series: `-0.32`
  - 5-movie series: `-0.46`

###  Trend Visualization  
- Plotted **average IMDb rating vs. sequel order** for each group (2, 3, 4, 5-movie series) on a single lineplot.

---

##  Key Observations

- **Negative correlations** suggest that, on average, sequels tend to perform worse than their predecessors.
- The trend lineplot clearly visualizes the average rating drop across sequel numbers for each group.

---

##  Dependencies

- Python 3 (Jupyter Notebook)
- Libraries:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `seaborn`
  
---


