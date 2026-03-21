# 💊 Digital Prescription Analysis

An end-to-end **ETL and analytics project** built with **Python, MySQL, Pandas, SQLAlchemy, and Matplotlib** to process prescription data from CSV files, clean and transform it, load it into a relational database, and generate business insights through SQL analysis and visualizations.

This project demonstrates how raw healthcare-related data can be transformed into a structured analytical system for better reporting, monitoring, and decision-making.

---

## 📌 Project Overview

**Digital Prescription Analysis** is designed to manage and analyze prescription records in a structured way.  
The pipeline follows the **ETL process**:

- **Extract** data from multiple CSV datasets
- **Transform** the data through cleaning and preprocessing
- **Load** the processed data into a MySQL database
- **Analyze** the data using SQL queries and visual reports

The project focuses on prescription-related entities such as:

- **Doctors**
- **Patients**
- **Medicines**
- **Prescriptions**

---

## 🛠️ Tech Stack

- **Python**
- **Pandas**
- **MySQL**
- **SQLAlchemy**
- **mysql-connector-python**
- **Matplotlib**
- **urllib.parse**

---

## 📂 Datasets Used

The project uses four input datasets:

1. **Doctors**
2. **Patients**
3. **Medicines**
4. **Prescriptions**

These datasets are read from CSV files and processed through the ETL pipeline.

---

## 🔄 ETL Workflow

## 1. Extract

The extraction phase reads data from the CSV datasets into Python using **Pandas**.

### Files loaded:
- `doctors.csv`
- `patients.csv`
- `medicines.csv`
- `prescriptions.csv`

This step forms the raw input layer of the project.

---

## 2. Transform

The transformation phase focuses on improving data quality and preparing the datasets for database loading and analytics.

### Data cleaning operations performed:
- Removed duplicate records using `drop_duplicates()`
- Handled missing values using `fillna()`
- Converted date columns into proper datetime format using `to_datetime()`
- Standardized column formats where required
- Prepared the datasets for relational storage

This step ensures the data is clean, consistent, and ready for downstream use.

---

## 3. Load

The load phase stores the cleaned data into a MySQL database.

### Database activities performed:
- Established connection to MySQL using **SQLAlchemy**
- Created the target database using SQL execution methods
- Created required tables using SQL queries
- Loaded cleaned datasets into MySQL using `to_sql()`

This step converts the cleaned flat-file data into a structured relational database model.

---

## 🗄️ Database Design

The MySQL database is designed to store healthcare prescription records in a normalized format.

### Core tables:
- **doctors**
- **patients**
- **medicines**
- **prescriptions**

This structure helps maintain organized relationships between doctors, patients, medicines, and issued prescriptions.

---

## 📊 Business Analysis & Visualizations

After loading the data into MySQL, analytical SQL queries and visualizations are used to generate insights.

### Key analyses performed:

#### 1. Most Prescribed Medicines
Identifies the medicines that are prescribed most frequently.

<img width="860" height="486" alt="Most Prescribed Medicines" src="https://github.com/user-attachments/assets/a2b2803e-46e8-4ea0-a9fb-c2d3f278be30" />

---

#### 2. Doctors by Prescription Volume
Shows which doctors generate the highest number of prescriptions.

<img width="861" height="482" alt="Doctors by Prescription Volume" src="https://github.com/user-attachments/assets/2f11d541-061f-4aa0-8aca-f43a4978f4e3" />

---

#### 3. Gender-wise Prescription Distribution
Analyzes prescription distribution based on patient gender.

<img width="442" height="352" alt="Gender-wise Prescription Distribution" src="https://github.com/user-attachments/assets/98b79fab-4aec-4a8c-868b-a826e19f958d" />

---

#### 4. Age Group vs Number of Prescriptions
Shows how prescriptions are distributed across different patient age groups.

<img width="892" height="480" alt="Age Group vs Number of Prescriptions" src="https://github.com/user-attachments/assets/585a8c68-f0a7-41d6-ad21-5c9d4083a5c7" />

---

#### 5. Doctor Prescription Count (Outlier Detection)
Highlights unusually high or low prescription activity among doctors.

<img width="893" height="481" alt="Doctor Prescription Count Outlier Detection" src="https://github.com/user-attachments/assets/40e5f504-36d5-4c93-9155-9b0797078bf8" />

---

#### 6. Daily Prescription Trend Over Time
Tracks prescription activity over time to identify trends and fluctuations.

<img width="883" height="435" alt="Daily Prescription Trend Over Time" src="https://github.com/user-attachments/assets/bb81e6b9-105a-4732-909b-28787b946267" />

---

#### 7. Missing Data Impact Analysis (Before vs After Cleaning)
Compares missing data levels before and after the cleaning process.

<img width="886" height="607" alt="Missing Data Impact Analysis" src="https://github.com/user-attachments/assets/0dec1388-9ad8-462e-be6b-65b06e79742b" />

---

## ✅ Features

- End-to-end ETL workflow
- Multi-file CSV ingestion
- Data cleaning and preprocessing
- MySQL database integration
- Relational table creation
- SQL-based analytical queries
- Visual reporting using Matplotlib
- Healthcare-oriented business insights

---

## 📁 Project Structure

```bash
Digital-Prescription-Analysis/
│
├── data/
│   ├── doctors.csv
│   ├── patients.csv
│   ├── medicines.csv
│   └── prescriptions.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── scripts/
│   ├── extract.py
│   ├── transform.py
│   ├── load.py
│   └── analysis.py
│
├── visuals/
│   ├── top_medicines.png
│   ├── doctor_volume.png
│   ├── gender_distribution.png
│   ├── age_group_analysis.png
│   ├── outlier_detection.png
│   ├── daily_trend.png
│   └── missing_data_impact.png
│
├── requirements.txt
└── README.md
