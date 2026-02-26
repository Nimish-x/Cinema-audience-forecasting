# Cinema Audience Forecasting

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data_Processing-150458?logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-blueviolet)

## Overview

This repository contains my approach and analysis for the **Cinema Audience Forecasting** challenge. The main objective of this project is to accurately predict cinema audience attendance using historical ticketing and visitation data. By leveraging exploratory data analysis (EDA), feature engineering, and robust machine learning regression models, we aim to forecast movie theater turnouts. Understanding audience turnout helps cinemas optimize staff scheduling, manage inventory, and plan better marketing strategies.

## The Problem

Predicting theater attendance is challenging due to the high volatility driven by various factors such as:
- Day of the week (weekends vs. weekdays)
- Holidays and special events
- Movie genres and popularity
- Seasonal trends

The goal is to build a predictive model that can effectively capture these dynamics and forecast the total number of visitors (`audience_count`) for specific theater locations on given dates.

## Dataset

The dataset (provided via the Kaggle competition) includes several historical data files related to cinema bookings and visits:
- `booknow_visits.csv` (Primary training data): Contains historical daily audience counts for each booked theater ID.
- `sample_submission.csv`: The required format for forecasting the test set.
- **Relational Data**: `movie_theater_id_relation.csv`, `date_info.csv`, `booknow_theaters.csv`, `cinePOS_booking.csv`, `cinePOS_theaters.csv`, `booknow_booking.csv`

**Key Features Explored:**
- `book_theater_id`: Unique identifier for the movie theater.
- `show_date`: The date of the cinematic showing.
- `audience_count`: The target variable to predict (number of visitors).

## Tools & Libraries

The project is implemented in Python and makes use of the following core tools in the Jupyter Notebook environment:
- **Pandas & NumPy**: For efficient dataset loading, data manipulation, and feature engineering.
- **Seaborn & Matplotlib**: To create informative visualizations, allowing us to spot trends like weekly attendance seasonality.
- **Jupyter Notebook**: For an interactive and structured analytical workflow.

## Repository Structure

```
├── Cinema_Audience_Forecasting.ipynb   # Main Jupyter Notebook containing data loading, EDA, and model building
├── README.md                           # Project documentation (this file)
└── .gitignore                          # Standard Python/Jupyter gitignore
```

## Exploratory Data Analysis (EDA) Highlights

Our initial EDA reveals strong repeating patterns in the audience count:
- **Weekly Trends**: There is a clear surge in audience count toward the weekend (Friday, Saturday, and Sunday) compared to regular weekdays.
- Visualizations built with Seaborn effectively demonstrate these patterns.

## How to Use

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Nimish-x/Cinema-audience-forecasting.git
   cd Cinema-audience-forecasting
   ```

2. **Run the Notebook:**
   Launch the notebook to see the data processing steps and visualizations.
   ```bash
   jupyter notebook Cinema_Audience_Forecasting.ipynb
   ```
   *(Ensure you have the Kaggle dataset downloaded and accessible at the specified input path to run the cells properly).*

---
*Feel free to star ⭐ this repository if you find the analysis helpful! If you have any questions or suggestions, please open an issue or reach out.*
