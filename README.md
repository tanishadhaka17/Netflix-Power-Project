# Netflix Content Analysis Dashboard (Power BI)

A data analytics project completed as part of my Unified Mentor Data Analyst Internship, focused on analyzing Netflix’s global catalog using Power BI, Power Query, and DAX.

## 📌 Project Overview

This Power BI dashboard provides a comprehensive exploration of Netflix’s content library. It includes insights on global content distribution, genre popularity, ratings, release-year trends, and country-level contributions.
The goal of the project is to convert raw Netflix data into meaningful, actionable visual insights through interactive BI reporting.

## ✅ Key Features
1. Global Content Map

Visual representation of Netflix titles across countries, showing concentration of content production.

2. Movies vs. TV Shows Distribution

Donut chart breaking down the share of Movies and TV Shows.

3. Release Year Trends

Line chart displaying the number of titles released each year, highlighting growth patterns.

4. Top 5 Countries by Content Count

Bar chart ranking countries contributing the highest number of titles.

5. Ratings Breakdown

Comparison of maturity ratings like TV-MA, TV-14, PG-13, etc.

6. Duration Analysis

Distribution of movie durations and TV show seasons.

7. Genre Segmentation

Treemap visualization showcasing top genres.

8. Dynamic Filters

Includes slicers for:

Release Year

Content Type (Movie/TV Show)

Ratings

## 🧹 Data Cleaning & Transformation (Power Query)

The dataset was cleaned and standardized using Power Query. Key transformations:

Removed duplicates and null records

Standardized country and genre fields

Split duration into numeric (minutes/seasons) and type

Converted release_year to numeric

Trimmed and formatted text columns

Ensured consistent categorical classifications

## 🧮 DAX Measures Used

Some examples of analytical measures:

Total Titles = COUNTROWS('netflix_titles')

Total Movies = CALCULATE(COUNTROWS('netflix_titles'), 'netflix_titles'[type] = "Movie")

Total TV Shows = CALCULATE(COUNTROWS('netflix_titles'), 'netflix_titles'[type] = "TV Show")

Titles by Rating = COUNT('netflix_titles'[rating])


(More DAX measures can be added as needed.)

## 📊 Dashboard Visuals Included

World Map

Donut Chart: Movie vs. TV Show

Line Graph: Yearly Trends

Horizontal Bar Chart: Top Countries

Bar Chart: Ratings

Treemap: Genres

Duration Count Visual

## 📁 Project Structure
Netflix-PowerBI-Dashboard
│── netflix_titles.csv
│── Netflix_Dashboard.pbix
│── README.md
│── /images (optional screenshots)

## 🛠 Tools & Technologies
Tool	Purpose
Power BI	Dashboard creation & data modeling
Power Query	Data cleaning & transformation
DAX	Calculated measures
Excel / CSV	Source dataset
## 📈 Key Insights from the Dashboard

Movies dominate the Netflix catalog.

TV-MA is the most frequently assigned maturity rating.

Post-2015 shows a significant rise in new content.

A few countries contribute disproportionately more titles.

Genres like Action, Drama, and Comedy appear most frequently.

## 📥 How to Use

Clone or download the repository.

Open the .pbix file in Power BI Desktop.

Ensure the dataset path is correctly linked.

Explore the interactive dashboard using slicers and drilldowns.

👩‍💻 Author

Tanisha
Data Analyst Intern – Unified Mentor
LinkedIN: www.linkedin.com/in/tanisha-dhaka
Github: 
