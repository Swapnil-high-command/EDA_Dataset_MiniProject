# EDA_Dataset_MiniProject
Exploratory Data Analysis (EDA) Project  This project dives deep into understanding and visualizing data through Exploratory Data Analysis (EDA). The goal is to uncover hidden patterns, relationships, and trends that can drive better decision-making and future modeling. Using Python’s powerful data analysis libraries like Pandas, NumPy,Matplotlib 
# Zomato Dataset: Exploratory Data Analysis (EDA)

## About This Project

This repository contains a Jupyter Notebook performing an in-depth Exploratory Data Analysis (EDA) on the Zomato dataset. The objective is to analyze restaurant data to uncover patterns and insights related to restaurant ratings, locations, cuisines, and services across different countries.

## Datasets Used

The analysis is based on two data files:
* `zomato.csv`: The primary dataset containing detailed information about restaurants, including their location, average cost, ratings, and services.
* `Country-Code.xlsx`: A mapping file used to associate the `Country Code` in the main dataset with the corresponding country name.

## Analysis and Visualizations

The notebook systematically explores the data by performing the following steps:

1.  **Data Loading and Cleaning:**
    * Loading the `zomato.csv` and `Country-Code.xlsx` files.
    * Inspecting the data's structure, columns, and data types (`.info()`, `.describe()`, `.shape()`).
    * Checking for and visualizing missing values using a `seaborn` heatmap.

2.  **Feature Engineering:**
    * Merging the main DataFrame with the country code data to add a human-readable `Country` column.

3.  **Geographical Analysis:**
    * Identifying the top 3 countries with the most restaurant listings using `value_counts()`.
    * **Visualization:** A pie chart showing the distribution of Zomato's presence, highlighting that **India** has the maximum number of listings, followed by the **USA** and **UK**.

4.  **Rating Analysis:**
    * Grouping data by `Aggregate rating`, `Rating color`, and `Rating text` to understand the rating system.
    * **Visualization:** A bar plot showing the count for each aggregate rating, color-coded by the rating text (e.g., "Excellent", "Good", "Average").
    * **Observation:** A high number of restaurants have "Not Rated" (a rating of 0.0).
    * **Observation:** The majority of rated restaurants fall within the "Average" range (2.5 - 3.4).

5.  **Service and Location Analysis:**
    * **Zero Ratings:** Investigating which country has the most "Not Rated" restaurants (India).
    * **Currency Mapping:** Identifying the currency used by each country.
    * **Online Delivery:** Determining which countries have online delivery options (India and UAE).
    * **Top Cities:** Creating a pie chart to show the top 5 cities with the most restaurant listings.

## Key Insights

This analysis uncovered several key insights:

* **India Dominates:** The vast majority of Zomato's listings and transactions are from India (over 8,600 listings).
* **"Not Rated" is Common:** A significant number of restaurants (over 2,100) have a 0.0 rating, with the majority of these located in India.
* **Online Delivery is Limited:** Online delivery services are primarily available only in India and the UAE.
* **Top Cities:** New Delhi has the most listings by a large margin, followed by Gurgaon and Noida.

## Technologies Used

* **Python**
* **Pandas:** For data manipulation and analysis.
* **NumPy:** For numerical operations.
* **Matplotlib:** For creating static, animated, and interactive visualizations.
* **Seaborn:** For high-level statistical data visualization.
* **Jupyter Notebook:** For interactive analysis and presentation.

## How to Run

To run this project on your local machine:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/](https://github.com/)[YOUR-USERNAME]/[YOUR-REPOSITORY-NAME].git
    ```

2.  **Navigate to the project directory:**
    ```bash
    cd [YOUR-REPOSITORY-NAME]
    ```

3.  **Install the required libraries:**
    ```bash
    pip install pandas numpy matplotlib seaborn openpyxl
    ```

4.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook 1-eda-feature-engineering.ipynb
    ```
