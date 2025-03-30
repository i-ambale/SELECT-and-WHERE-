# UN Data Analysis: Access to Basic Services

This repository contains a Jupyter Notebook that connects to a local MySQL database (`united_nations`) and explores access to managed drinking water services across different countries using SQL queries.

## 📚 Project Overview

We query and analyze data from the `Access_to_Basic_Services` table, focusing on metrics like percentage of population with access to safely managed drinking water, sorted and filtered by specific conditions.

## 🛠️ Technologies Used

- Python 3
- Jupyter Notebook
- MySQL
- SQLAlchemy
- PyMySQL

## 📁 Files

- `UN_Data_Analysis.ipynb` – Jupyter notebook containing SQL queries, database interaction, and analysis.
- `code_editor.xml` – A dark theme configuration file for the MySQL Workbench code editor.
- `README.md` – Project documentation (this file).

## 📊 Sample SQL Queries

Here are a few SQL snippets used in the notebook:

```sql
-- Display access to drinking water for 2020
SELECT
    Country_name,
    Time_period,
    Pct_managed_drinking_water_services AS pct_access_to_water
FROM
    access_to_basic_services
WHERE
    Time_period = 2020
LIMIT 10;
```
---
⚙️ Setup Instructions
1. Clone this repository:
  ```
  git clone https://github.com/your-username/un-data-sql.git
  ```

2. Start your MySQL server and ensure the united_nations database is running.

3. Open UN_Data_Analysis.ipynb in Jupyter Lab or Notebook.

4. Update your SQL connection string if necessary:
  ```
   %sql mysql+pymysql://root:<your-password>@localhost:3306/united_nations
  ```
5. Run the notebook cells to explore and analyze the data.
---
📌 License
This project is for educational use. Attribution is appreciated but not required.
---
🙌 Acknowledgments
ALX Africa – For support and mentorship

United Nations – For the publicly available datasets
---
Happy querying! 🧠📈

Let me know if you want it tailored more for class submission, a personal portfolio, or public open-source usage.

