# Netflix ETL & Data Analysis Project

This project demonstrates a complete **ETL (Extract, Transform, Load)** process using **Python**, **MySQL**, and **Pandas**, followed by basic exploratory data analysis on the Netflix dataset.

## Features

- Extract data from a CSV file (`netflix_titles.csv`)
- Load data into a MySQL database table (`netflix_raw`)
- Run SQL queries for data transformation (optional SQL script provided)
- Perform basic data analysis using Python (e.g., missing values, description lengths, filters)

## Tools & Technologies

- Python 3.x
- Pandas
- SQLAlchemy
- MySQL (via `mysql-connector-python`)

## Folder Structure

SQL-ETL-Netflix/ ├── data_extract.py # Python script to load data into MySQL ├── data_analysis.sql # SQL queries for analysis (optional) ├── netflix_raw.sql # SQL schema for table creation (optional) ├── netflix_titles.csv # Source dataset └── README.md


## How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/Jayantk24/ETL-Data-Analysis.git
cd ETL-Data-Analysis

2. Install Dependencies

pip install pandas sqlalchemy mysql-connector-python

3. Setup MySQL
Create a database named netflix_db

Update your MySQL password in data_extract.py:

engine = sal.create_engine('mysql+mysqlconnector://root:your_password@localhost:3306/netflix_db')

4. Run the ETL Script

python data_extract.py



Output Examples

Total null values per column
Longest description length
All rows where show_id == 's5023'

Dataset Source
Netflix Titles Dataset: Kaggle - Netflix Movies and TV Shows

Author
Jayant Kasturia