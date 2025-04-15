##  Research Metadata Analysis Using Springer Nature Open Access API  
###  A Big Data Analytics Project for Research Information Management  
   
________________________________________
#### 🔹 Overview
This project demonstrates Big Data Analytics in Research Information Management by:  

  
✅ Mining Open Access research metadata using the Springer Nature API  
✅ Cleaning & structuring metadata for efficient analysis  
✅ Storing data in PostgreSQL for structured querying  
✅ Performing Exploratory Data Analysis (EDA) to identify trends in scientific research  
✅ The project was created with a Jupyter notebook, the file is available in this repo  
  
 Primary Goal:  
To analyze climate change research trends, discover top authors, journals, and keywords, and build a structured research data pipeline.  
________________________________________
#### 🔹 Project Workflow  
Step 1: Data Ingestion & API Integration  
🔹 Extract research metadata (titles, authors, journals, subjects) from the Springer Nature Open Access API.  
🔹 Store raw data in JSON/CSV format for processing.  
Step 2: Data Cleaning & Transformation  
🔹 Flatten nested JSON fields (e.g., authors, subjects, URLs).  
🔹 Handle missing values and ensure structured data format.  
Step 3: Storing Data in PostgreSQL  
🔹 Define a PostgreSQL schema for structured storage.  
🔹 Insert cleaned metadata into PostgreSQL tables.  
🔹 Verify data integrity using SQL queries.  
Step 4: Exploratory Data Analysis (EDA)  
🔹 Analyze research publication trends over time.  
🔹 Identify top journals, most cited authors, and key topics.  
🔹 Generate visualizations using Pandas & Matplotlib.  
Step 5: Deployment & GitHub repository  
🔹 Showcase project results on GitHub.  
________________________________________
#### 🔹 Technologies Used  
Programming & Scripting:  
•	Python (pandas, matplotlib, psycopg2)  
•	Jupyter Notebook for interactive data analysis  
Database & Storage:  
•	PostgreSQL for structured research metadata storage  
•	GitHub for project showcase  
APIs & Data Sources:  
•	Springer Nature Open Access API for metadata extraction   
•	GitHub for project version control & hosting  
________________________________________
#### 🔹 Setup & Installation  
Step 1: Clone the Repository  
git clone https://github.com/HannaKuzmina2024/mpdl-project.git  
cd  mpdl-project  
Step 2: Set Up a Virtual Environment  
python -m venv venv  
source venv/bin/activate    # Mac/Linux  
venv\Scripts\activate       # Windows  
Step 3: Install Dependencies  
pip install -r requirements.txt  
Step 4: Set Up PostgreSQL Database  
1.	Start PostgreSQL (pgAdmin or CLI).  
2.	Create a new database:   
3.	CREATE DATABASE research_metadata;  
4.	Create the required table:   
5.	CREATE TABLE research_articles (

id SERIAL PRIMARY KEY,  
content_type TEXT,  
identifier TEXT UNIQUE,  
language TEXT,  
url TEXT,  
title TEXT,  
creators TEXT,  
publication_name TEXT,  
subjects TEXT  
    
);  
Step 5: Configure API Key & Database Credentials  
1.	Create a .env file:   
2.	touch .env  
3.	Add your credentials:   
4.	SPRINGER_API_KEY=your-api-key-here  
5.	POSTGRES_PASSWORD=your-database-password-here  
   
Step 6:  Open Jupyter Notebook and execute the cells.  
(I am using Jupyter notebook in VS.code)  

________________________________________
 
🔹 Most Frequent Research Journals    


![mostfrequentjournals](https://github.com/user-attachments/assets/7af0914d-55c1-4b5d-b525-debd56893320)

🔹 Most Published Authors    


![mostpublished authors](https://github.com/user-attachments/assets/40f8c1a8-ec14-406a-b1d1-898c7dfa26da)

🔹 Example Visualization


![top10](https://github.com/user-attachments/assets/48e17fbe-9b73-447f-9926-2143a4a6a653)





