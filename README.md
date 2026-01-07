Netflix Movies Data Analysis
A comprehensive data analysis project that cleans, analyzes, and visualizes Netflix movie data using Python and Power BI to extract actionable insights about content trends, ratings, and genre popularity.

📊 Project Overview:

This project transforms raw Netflix movie data into meaningful insights through systematic data cleaning, exploratory data analysis (EDA), and interactive visualizations. The analysis reveals patterns in movie popularity, genre distribution, release trends, and audience ratings.

✨ Features:

Data Cleaning & Preprocessing: Handled missing values, removed duplicates, and standardized date formats

Exploratory Data Analysis: Statistical analysis of movie ratings, popularity scores, and vote counts

Genre Analysis: Breakdown and visualization of genre distribution across the dataset

Popularity Segmentation: Categorized movies into Famous, Average, Below Average, and Not Popular tiers

Interactive Dashboard: Power BI dashboard for dynamic data exploration

Trend Analysis: Release year patterns and temporal trends in movie production

🛠️ Tech Stack
Programming & Libraries:

Python 3.x

pandas - Data manipulation and cleaning

NumPy - Numerical operations

Matplotlib - Data visualization

Seaborn - Statistical data visualization

Business Intelligence:

Power BI - Interactive dashboard creation

Data Format:

CSV - Data storage and exchange

📁 Project Structure:
text
netflix-analysis/
│
├── mymoviedb.csv              # Original raw dataset
├── cleaned_mymoviedb.csv      # Cleaned and processed dataset
├── Netflix-Analysis.ipynb     # Jupyter notebook with analysis
└── README.md                  # Project documentation
📈 Dataset Information
The dataset contains 9,827 movies with the following key attributes:

Column	Description
Release_Date	Movie release year
Title	Movie title
Popularity	Popularity score metric
Vote_Count	Total number of user votes
Vote_Average	Categorized rating (Famous, Average, Below Average, Not Popular)
Genre	Movie genre(s) - exploded for multi-genre entries

🔍 Key Insights:

Data Cleaning Process-
Date Conversion: Transformed Release_Date from full date format to year-only format

Column Removal: Dropped non-essential columns (Overview, Original_Language, Poster_Url)

Rating Categorization: Created Vote_Average categories based on popularity and vote thresholds:

Famous: High vote count (>800)

Average: Moderate metrics

Below Average: Lower engagement

Not Popular: Minimal votes

Genre Normalization: Split multi-genre entries into individual rows for granular analysis

Missing Value Treatment: Handled null values in critical fields

Statistical Summary
Average Popularity Score: 40.33

Average Vote Count: 1,393 votes per movie

Average Rating: 6.44/10

Release Year Range: 1959 - 2023

Total Genres Represented: 20+ unique genres

Most Common Genres: Drama, Comedy, Action, Adventure, Thriller

🚀 Getting Started
Prerequisites
bash
python >= 3.7
pandas >= 1.3.0
numpy >= 1.21.0
matplotlib >= 3.4.0
seaborn >= 0.11.0

📊 Analysis Workflow:

1. Data Loading & Inspection
python
import pandas as pd
df = pd.read_csv('mymoviedb.csv', lineterminator='\n')
df.head()
df.info()
df.describe()
2. Data Cleaning
Converted Release_Date to year format

Removed unnecessary columns

Categorized popularity ratings

Handled missing values

Normalized genre data

3. Exploratory Data Analysis
Distribution analysis of popularity, votes, and ratings

Genre frequency analysis

Temporal trends in movie releases

Correlation analysis between variables

4. Visualization
Bar charts for genre distribution

Time series plots for release trends

Scatter plots for popularity vs. ratings

Heatmaps for correlation matrices

5. Power BI Dashboard
Created interactive dashboard with:

Genre breakdown visualizations

Release year trends

Popularity distribution charts

Top-rated movies filters

Vote count analytics

📸 Sample Visualizations
The analysis includes multiple visualization types:

Genre Distribution: Bar charts showing frequency of each genre

Popularity Trends: Line graphs tracking popularity over time

Rating Analysis: Histograms of vote averages and distributions

Vote Count Patterns: Scatter plots correlating votes with ratings

💡 Use Cases
Content Strategy: Identify popular genres for content acquisition

Audience Insights: Understand viewer preferences and engagement patterns

Trend Forecasting: Predict future content trends based on historical data

Performance Benchmarking: Compare movie performance metrics

Market Analysis: Analyze competitive landscape in streaming content

🔮 Future Enhancements
 Add sentiment analysis on movie descriptions

 Implement machine learning models for popularity prediction

 Include regional/language-based analysis

 Add more granular time-series forecasting

 Integrate real-time data updates

📝 Lessons Learned
Importance of systematic data cleaning for accurate analysis

Value of categorical segmentation for pattern identification

Power of combined Python + Power BI approach for comprehensive analysis

Genre normalization crucial for accurate frequency analysis
