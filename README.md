# Loan Risk Analytics & ETL Pipeline

This project is a comprehensive **ETL (Extract, Transform, Load)** pipeline designed to process massive credit risk datasets (Lending Club) and transform them into actionable insights via an interactive Power BI dashboard.

## 🎯 Project Objective
The goal of this project is to manage and analyze large-scale datasets (over 9 million records) to evaluate borrower credit risk. The pipeline efficiently transforms raw data into a structured, queryable format, enabling intelligent reporting and risk assessment.

## 🚀 Key Features
*   **Memory-Efficient Processing:** Utilizes Python’s chunking technique to process millions of rows without hitting `MemoryError` limits.
*   **Automated ETL Pipeline:** Handles extraction of Accepted and Rejected loans, performs data cleaning, and loads the data into an optimized SQLite database.
*   **BI Integration:** Seamlessly connects the cleaned output to Power BI for visual analysis of loan approval rates and key risk metrics (FICO Score & DTI Ratio).
*   **Database Optimization:** Implements `PRAGMA` settings in SQLite to significantly accelerate write operations during the loading phase.

## 🛠 Tech Stack
*   **Programming:** Python (Pandas, NumPy)
*   **Database:** SQLite
*   **Visualization:** Power BI
*   **Tools:** Jupyter Notebook, Git

## 📈 Project Workflow
1.  **Data Extraction:** Reading large CSV files using chunking to maintain system stability.
2.  **Transformation:** Dropping unnecessary columns, handling missing values, and creating risk labels.
3.  **Loading:** Efficiently writing the processed data into `loan_risk.db`.
4.  **Dashboarding:** Visualizing approval rates and loan boundary analysis using the integrated dataset.

## ⚙️ How to Run
1. Place your raw CSV files in the project directory.
2. Execute the Python notebook to build the `loan_risk.db` database.
3. Connect the generated database file to Power BI as a data source to interact with the dashboard.
