# Customer Shopping Behavior Analysis

## Project Overview

This project demonstrates an end-to-end data analysis workflow using Python, MySQL, and Power BI. Python in Anaconda/Jupyter Notebook is used to prepare and transform the data, MySQL is used to store the prepared data and answer business questions with SQL queries, and Power BI is used to build an interactive dashboard.

## Tools and Technologies

- **Python** — data preparation and transformation
- **Anaconda and Jupyter Notebook** — Python environment and notebook workflow
- **MySQL** — storing and querying the prepared data
- **MySQL Workbench** — writing and running SQL queries (if used in this project)
- **Microsoft Power BI Desktop** — dashboard and visual reporting

## Project Workflow

1. **Inspect the data:** review the source data, its columns, data types, and quality issues.
2. **Transform the data with Python:** perform the cleaning and transformations recorded in the notebook.
3. **Load the prepared data into MySQL:** import the transformed data into the database and confirm that the table and row counts look correct.
4. **Analyse with SQL:** run SQL queries to answer questions about customers and shopping behaviour.
5. **Build the Power BI dashboard:** connect Power BI to the prepared data and present the results with charts, cards, and filters.

## Repository Contents

Use this as the suggested structure; change folder and file names to match the files you actually upload.

```text
Customer-Shopping-Behavior-Analysis/
├── README.md
├── notebooks/
│   └── data_cleaning_and_transformation.ipynb
├── sql/
│   └── analysis_queries.sql
├── powerbi/
│   └── customer_shopping_dashboard.pbix
├── images/
│   └── dashboard_preview.png
└── data/
    └── (include only data you are permitted to share)
```

## How to Reproduce the Analysis

1. Download or obtain the dataset from its original source and check its licence and sharing conditions.
2. Open the Jupyter notebook in Anaconda/Jupyter and run the cells in order. Update any file paths so they point to your local dataset.
3. Import the transformed data into your local MySQL database using the process documented in the notebook or your SQL scripts.
4. Open the SQL file in MySQL Workbench (or another MySQL client), select the correct database, and run the queries.
5. Open the Power BI `.pbix` file in Power BI Desktop. Update its data-source settings to match your own local MySQL connection, then refresh the data.

**Note:** Database names, table names, file paths, and connection settings may differ on another computer. Do not put database passwords or other credentials in the notebook, SQL file, README, or GitHub repository.

## Business Questions and Findings

Document the questions answered by your SQL queries and Power BI visuals here. Add only findings that you have verified from your actual results. For example, you may describe customer segments or purchasing patterns if those are part of your analysis.

- **Question 1:** Add the business question and a brief result.
- **Question 2:** Add the business question and a brief result.
- **Question 3:** Add the business question and a brief result.

## Dashboard Preview

Add a screenshot of your finished Power BI dashboard to `images/dashboard_preview.png`, then replace this note with the image embed below:

```markdown
![Power BI dashboard preview](images/dashboard_preview.png)
```

## Data and Privacy

- Credit the dataset's original source and respect its licence or terms of use.
- Do not upload passwords, `.env` files, private customer information, or confidential data.
- If the dataset is too large or cannot legally be redistributed, document where it came from instead of committing the data file.
- Before publishing, review notebook outputs as well as the code: outputs can contain personal data, connection details, or other sensitive information.

## Author

**Your Name**  
Add your LinkedIn or portfolio link here, if you want to share it.
