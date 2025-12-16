# Zomato — Data Cleaning & Exploratory Data Analysis

Data cleaning and exploratory analysis on the Zomato restaurants dataset using pandas.  
This repo contains the notebook I used to clean the data, inspect features, and produce the main visualizations in `figures/`.

---

## Dataset
- Source: Zomato Restaurants Dataset (Kaggle)  
- Link: https://www.kaggle.com/datasets/shrutimehta/zomato-restaurants-data  
- Note: The raw dataset is not included in this repository due to size. Place the downloaded CSV as `data/zomato.csv` before running the notebook.

---

## How to run
1. Download the Zomato dataset from Kaggle.  
2. Create a `data/` folder in the project and put the CSV there as `data/zomato.csv`.  
3. (Optional) Create and activate a virtual environment:
  ```bash
python -m venv venv
# mac / linux
source venv/bin/activate
# windows (PowerShell)
venv\Scripts\Activate.ps1


---


## Install dependencies:

pip install -r requirements.txt

---


## Open zomato_code.ipynb in Jupyter or Colab and run the cells top → bottom. For a quick demo, use a small sample file data/sample_zomato.csv.

---

## Project structure
zomato-dataset-eda/
├── zomato_code.ipynb
├── figures/
├── README.md
└── requirements.txt


---

## Data cleaning steps

The following cleaning steps were performed before analysis:

Handled missing and invalid values in rating and cost columns.

Removed duplicate records.

Converted rating and cost columns to usable numerical formats.

Standardized cuisine and city-related fields.

Checked correlations among numerical features.

---

## Exploratory Data Analysis

The EDA focuses on understanding restaurant distribution, customer ratings,
pricing patterns, and cuisine popularity across different cities.

Key analyses include:

Distribution of restaurants across cities

Most common cuisines and cities

City-wise median ratings

Cost comparison across cities

Relationship between cost and ratings

Correlation between numerical variables

---

## Key insights

Some important insights obtained from the analysis:

A small number of cities dominate the dataset, with cities like New Delhi having a significantly higher number of restaurants compared to others.

Popular cuisines are highly concentrated, indicating that a few cuisines are repeatedly preferred across different regions.

Higher cost does not necessarily guarantee better ratings, suggesting that customer satisfaction depends on more than just pricing.

Certain cities consistently show higher median ratings, highlighting regional differences in food quality or customer expectations.

Correlation analysis shows weak relationships between most numerical features, indicating that restaurant ratings are influenced by multiple independent factors.

Currency usage varies significantly, but most restaurants operate in a small set of commonly used currencies.

---

## Visualizations

The figures/ folder contains the most important plots from the analysis, including:

Correlation heatmap of numerical features

Top cities by number of restaurants

Top cuisines by frequency

Cities with highest median ratings

Costliest cities based on average cost

Restaurants with highest median ratings

These plots provide a quick visual summary of the dataset without running the notebook.

---

## Tools & libraries used

Python

Pandas, NumPy

Matplotlib, Seaborn

---

## Conclusion

This project demonstrates a complete workflow of data cleaning and exploratory
data analysis on a real-world dataset. It helped reinforce practical usage of
pandas, grouping operations, and visualization techniques commonly used in
data analysis tasks.




