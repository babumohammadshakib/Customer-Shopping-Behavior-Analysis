Customer Shopping Behavior Analysis

Project Overview

In this project, I analyzed customer shopping behavior using Python, MySQL, and Power BI. I used Python in Anaconda/Jupyter Notebook to explore, clean, and transform the dataset. I then loaded the prepared data into MySQL, used SQL queries to examine customer and purchase information, and built a dashboard in Power BI to present the data visually.

Tools and Technologies

- Python (Pandas): Data inspection, cleaning, and transformation
- Anaconda and Jupyter Notebook: Python environment and analysis workflow
- MySQL: Storage and querying of the prepared dataset
- MySQL Workbench: Writing and running SQL queries
- Microsoft Power BI Desktop: Interactive dashboard and visual reporting
  
Dataset

I used the Customer Shopping Trends Dataset from Kaggle.
- Source: Customer Shopping Trends Dataset on Kaggle
- Raw dataset size: 3,900 records and 18 columns
- Main information: Customer age and gender, purchased item and category, purchase amount, location, season, review rating, subscription status, shipping type, discounts, previous purchases, payment method, and purchase frequency.
  
Data Preparation with Python

I used the notebook customer_behavior.ipynb to inspect and prepare the dataset. The work includes:
1. Loading the CSV data with Pandas.
2. Reviewing the first records, column data types, summary statistics, and missing values.
3. Filling missing Review Rating values with the median rating for the corresponding product category. The original dataset had 37 missing values in this column.
4. Converting column names to lowercase and replacing spaces with underscores to make them easier to work with in SQL.
5. Checking Discount Applied and Promo Code Used for duplicate information and removing promo_code_used when the two columns matched across the dataset.
6. Creating an age_group feature using age quartiles.
7. Creating a purchase_frequency_days feature to represent purchase frequency as a number of days.

SQL Analysis with MySQL

I loaded the prepared dataset into a MySQL table named consumer in the customer_b database. The SQL script Customer_P_R.sql contains the queries used for the analysis.
The dataset supports analysis of customer demographics, spending, product categories, review ratings, subscriptions, discounts, shipping choices, payment methods, and purchase frequency.

Power BI Dashboard
<img width="1378" height="796" alt="image" src="https://github.com/user-attachments/assets/3dc9a7ef-7d25-4701-9a9b-583de291762a" />
I used Microsoft Power BI Desktop to create the dashboard saved as BI_Project.pbix. The dashboard is the visual reporting component of the project and complements the data preparation in Python and the SQL analysis in MySQL.
Project Files

All project files are currently stored in the repository's root directory:
Customer-Shopping-Behavior-Analysis/
├── README.md
├── .gitignore
├── customer_behavior.ipynb
├── customer_shopping_behavior.csv
├── Customer_P_R.sql
└── BI_Project.pbix

How to Reproduce the Project

1. Download or clone this repository and make sure Python, Anaconda/Jupyter Notebook, MySQL, and Power BI Desktop are available on your computer.
2. Open customer_behavior.ipynb in Jupyter Notebook and update the CSV file path to match your local copy of customer_shopping_behavior.csv.
3. Run the notebook cells in order to inspect and prepare the dataset.
4. Update the database connection settings in the notebook to match your own local MySQL setup. Use your own credentials locally; do not commit real passwords or other secrets to GitHub.
5. Run Customer_P_R.sql in MySQL Workbench after selecting the appropriate database.
6. Open BI_Project.pbix in Power BI Desktop. Update its data-source settings for your own environment if needed, then refresh the data.
Notes
- The notebook uses a local file path and local database settings that may need to be changed on another computer.
- The raw CSV is included for transparency and reproducibility. Please refer to the original Kaggle dataset page for its terms and usage conditions.
- The analysis and dashboard are based on the supplied dataset; results should be interpreted in the context of that dataset.
  
Author

Mohammad Shakib Babu
  https://www.linkedin.com/in/mohammad-shakib-babu-671643320/
