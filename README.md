# DP-203-Lab3
# 📊 DP-203_Lab3 - Transforming Data with Azure Synapse Serverless SQL Pools

This project is part of my learning journey through the Microsoft DP-203 Data Engineering course. In this lab, I learned how to analyze, transform, and store raw CSV data from a Data Lake as optimized Parquet files using Serverless SQL Pools in Azure Synapse Analytics.

---

## ✨ Lab Objective

The main focus of this exercise was to apply SQL transformations to raw data stored in a Data Lake. By using CETAS (Create External Table As Select), I was able to store the results directly in an external table.

---

## ⚙️ Requirements & Tools

- An active Azure account with sufficient permissions.
- Azure Synapse Analytics workspace connected to a Data Lake.
- Basic knowledge of SQL, PowerShell, and Azure Portal.
- GitHub repository dp-203 for the required setup scripts.

---

## 🛠️ Steps Completed

### 🔹 1. Setup & Source Files
- Used Azure Cloud Shell (PowerShell) to deploy the lab environment.
- Explored the CSV files located in the `sales/csv` folder via Synapse Studio.

### 🔹 2. Exploring Data with SQL
- Queried the file contents using `OPENROWSET` to view the structure.
- Analyzed sales data including Item, Quantity, OrderDate, UnitPrice, and TaxAmount.

### 🔹 3. Data Transformation
- Created a new dedicated database in Synapse Studio.
- Defined an external data source and file format for Parquet.
- Wrote a CETAS query to aggregate sales by product.

### 🔹 4. Custom Additions
- Added a computed column to extract the sales year (`YEAR(OrderDate)`).
- Filtered the data to include only rows with a valid EmailAddress.

### 🔹 5. Stored Procedure (Optional)
- Built a stored procedure to automate the transformation process.
- Results were written into the Data Lake as partitioned Parquet files.

### 🔹 6. Clean-up
- Deleted the resource group in Azure Portal to avoid unnecessary charges.


---

## 📚 Resources & Inspiration

- Microsoft Learn - DP-203
- Azure Synapse Analytics Documentation
- GitHub Repo: MicrosoftLearning/dp-203-Data-Engineer

---

## 🧠 What I Learned

This lab helped me:
- Apply the fundamentals of Serverless SQL Pools in a hands-on scenario.
- Understand the benefits of using Parquet for efficient storage.
- Perform SQL transformations on semi-structured data.
- Build data pipelines without relying on a dedicated Spark environment.

## Screenshots

<img width="782" alt="1" src="https://github.com/user-attachments/assets/a5f39439-090a-42dc-9e47-9faeace50680" />

<img width="1505" alt="2" src="https://github.com/user-attachments/assets/f8295b6d-922a-48b1-b91e-0b4925e32806" />

<img width="1504" alt="3" src="https://github.com/user-attachments/assets/ab211b0d-77fd-432c-b449-9de211a68065" />

<img width="1445" alt="4" src="https://github.com/user-attachments/assets/43182231-b49d-4b0f-9ca3-937526d252c3" />

<img width="1499" alt="5" src="https://github.com/user-attachments/assets/aa947591-72d9-43fc-8e9c-77c943893903" />


<img width="1512" alt="7" src="https://github.com/user-attachments/assets/3843fce1-4b2b-45e1-a737-8bf5f71fd879" />

<img width="1498" alt="8" src="https://github.com/user-attachments/assets/004558ee-4ec4-4a08-9873-7ec5208b260d" />

<img width="756" alt="9" src="https://github.com/user-attachments/assets/0344eadb-de96-4b5c-a2a6-45a6dde4d274" />


