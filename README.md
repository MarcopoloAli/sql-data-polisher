# MySQL Data Cleaning Project - Layoffs Dataset

## 📌 Project Overview
This project demonstrates how to clean and prepare a real-world dataset using **MySQL**.  
The dataset contains information about company layoffs, including:

- Company  
- Location  
- Industry  
- Total layoffs  
- Percentage laid off  
- Date  
- Stage  
- Country  
- Funds raised (in millions)  

The goal is to transform raw, messy data into a clean, analysis-ready format.

---

## 🛠️ Cleaning Steps
The following SQL operations were applied:

1. **Create a staging table**  
   - Work on a copy of the raw dataset to preserve original data.

2. **Remove duplicates**  
   - Ensure each company/date record is unique.

3. **Standardize text fields**  
   - Trim spaces, unify case (e.g., lowercase company names), and normalize country names.

4. **Handle missing values**  
   - Replace `NULL` values with defaults (e.g., 0 for percentages or funds raised).

5. **Convert date formats**  
   - Ensure all dates are stored in proper `DATE` format.

6. **Remove impossible values**  
   - Exclude records with negative layoffs or percentages greater than 100.

7. **Normalize categorical values**  
   - Example: unify "USA", "US", "United States" into a single value.

---

## 📂 Repository Structure
- `scripts/` → SQL scripts for cleaning  
- `data/` → Raw dataset (CSV or SQL dump)  
- `README.md` → Project documentation  

---

## 🚀 How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/mysql-data-cleaning-layoffs.git
