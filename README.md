# Web Server Log Analysis - Calgary HTTP Dataset

## 📘 Overview

This project is a Python-based analysis of the Calgary HTTP log dataset, which contains nearly one year of real HTTP requests made to the University of Calgary's Computer Science web server. The objective is to demonstrate the ability to clean, parse, and analyze raw web server logs using Python and pandas.



## 📂 Dataset Information

- **Source:** [Calgary HTTP Logs](https://ita.ee.lbl.gov/html/contrib/Calgary-HTTP.html)
- **Format:** Compressed `.gz` (ASCII text)
- **File Size:** 
  - Compressed: ~5.4 MB  
  - Uncompressed: ~52 MB  
- **Log Format:** Apache Common Log Format (CLF)



## 🔧 Tools Used

- **Python**
- **pandas**
- **Regular Expressions**
- **gzip**



## 🧹 Data Cleaning Highlights

- Handled `.gz` file reading with proper encoding (`latin1`)
- Parsed raw log lines using regex (Apache CLF)
- Converted timestamps to `datetime` objects
- Replaced missing byte values with `0`
- Flagged invalid filenames using `pd.NA`
- Extracted file extensions using regex
- Ensured correct data types (`int`, `datetime`, `string`)



## ✅ Analysis Tasks Implemented

| Task No. | Description                                      |
|----------|--------------------------------------------------|
| Q1       | Count of total log records                       |
| Q2       | Count of unique hosts                            |
| Q3       | Date-wise unique filename counts                 |
| Q4       | Number of 404 response codes                     |
| Q5       | Top 15 filenames resulting in 404 errors         |
| Q6       | Top 15 file extensions with 404 errors           |
| Q7       | Total bandwidth transferred per day (July 1995)  |
| Q8       | Hourly request distribution                      |
| Q9       | Top 10 most requested filenames                  |
| Q10      | HTTP response code distribution                  |



## 📁 Folder Structure

calgary-http-assessment/
├── analysis.ipynb # Main notebook with all logic
├── analysis.html # Exported HTML version of notebook
├── transcript.txt # Transcript of explanation video
└── README.md # This file


## 📌 Author

Sahil Talathi  
Post Graduate Diploma in Big Data Analytics  
Email: [sahiltalathi2@gmail.com]  
Location: Thane, India
