# Customer Shopping Behavior Analysis

## 📌 Project Overview

This project focuses on analyzing customer shopping behavior to understand purchasing patterns, customer preferences, and shopping trends.

The project uses a customer shopping dataset containing information about customer demographics, purchased items, purchase amounts, product categories, reviews, discounts, payment methods, and purchase frequency.

The objective is to prepare and analyze the data using Python and SQL, and present business information through a Power BI dashboard.

## 🎯 Project Objectives

- Understand customer shopping patterns and preferences.
- Clean and prepare the dataset for analysis.
- Handle missing values in customer review ratings.
- Create additional features to improve data analysis.
- Store the cleaned dataset in a MySQL database.
- Explore customer behavior and identify useful business insights.

## 🛠️ Tools and Technologies

- **Python:** Data cleaning and preprocessing
- **Pandas:** Data manipulation and analysis
- **NumPy:** Numerical operations
- **Jupyter Notebook:** Writing and executing Python code
- **MySQL:** Database storage and querying
- **SQLAlchemy and PyMySQL:** Connecting Python to MySQL
- **SQL:** Database analysis
- **Power BI:** Dashboard and data visualization

## 📂 Project Files

| File | Description |
|---|---|
| `customer_shopping_behavior.csv` | Customer shopping dataset |
| `Eda.ipynb` | Python notebook for data exploration and preprocessing |
| `Analysis.sql` | SQL queries for customer behavior analysis |
| `customer_behavior_dashboard.pbix` | Power BI dashboard |
| `Customer Shopping Behaviour Analysis.pdf` | Project analysis report |
| `README.md` | Project documentation |

## 📊 Dataset Description

The dataset contains **3,900 records and 18 original columns**.

Some important columns include:

- Customer ID
- Age and Gender
- Item Purchased
- Category
- Purchase Amount
- Location
- Season
- Review Rating
- Subscription Status
- Shipping Type
- Discount Applied
- Previous Purchases
- Payment Method
- Frequency of Purchases

## 🧹 Data Cleaning and Preparation

The Python notebook performs the following operations:

1. Loads the CSV dataset using Pandas.
2. Examines the dataset structure, data types, and descriptive statistics.
3. Identifies missing values in the `Review Rating` column.
4. Fills missing review ratings using the median rating within each product category.
5. Standardizes column names to lowercase and replaces spaces with underscores.
6. Renames `purchase_amount_(usd)` to `purchase_amount`.
7. Creates an `age_group` column to categorize customers into age groups.
8. Maps purchase frequencies to approximate numbers of days.
9. Checks whether `discount_applied` and `promo_code_used` contain identical values and removes the redundant column.
10. Loads the cleaned dataset into a MySQL table named `customer`.

## 🗄️ Database Integration

The cleaned dataset is transferred from Python to MySQL using SQLAlchemy and PyMySQL.

The data is stored in the `customer` table, allowing SQL queries to be executed on the prepared dataset.

## 📈 Analysis and Visualization

The project includes separate files for SQL analysis and Power BI visualization.

These components can be used to explore customer purchasing behavior, compare shopping patterns, and communicate findings through charts and reports.

## 💡 Learning Outcomes

- Understanding data exploration and preprocessing.
- Handling missing values using Pandas.
- Creating new columns through feature engineering.
- Working with categorical and numerical data.
- Connecting Python to a MySQL database.
- Transferring a Pandas DataFrame into a database table.
- Practicing SQL-based analysis and Power BI visualization.

## 🚀 How to Run

1. Download or clone the repository.
2. Install Python and the required libraries.
3. Place the CSV file in the appropriate working directory.
4. Open `Eda.ipynb` in Jupyter Notebook or VS Code.
5. Execute the notebook cells in order.
6. Install and configure MySQL.
7. Create the `customer_shopping` database and configure your database connection.
8. Run the SQL queries using a compatible MySQL client.
9. Open the `.pbix` file using Power BI Desktop.

**Required Python libraries:**

```bash
pip install pandas numpy sqlalchemy pymysql jupyter
```

**Note:** Update database credentials according to your local MySQL configuration. Do not publish passwords or other sensitive credentials.

## 👨‍💻 Author

**Abhishek Kumar**

GitHub: [abhishekkumar1906](https://github.com/abhishekkumar1906)

LinkedIn: [Abhishek Kumar](https://www.linkedin.com/in/abhishek-kumar-bb79a8320/)
