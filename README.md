# Wuzzuf Job Scraper

## 📌 Overview

This project is a web scraping script that extracts job listings from **Wuzzuf** based on a search query (e.g., *Data Engineer*).
It collects structured job data across multiple pages and exports the results into a CSV file.

---

## 🚀 Features

* Scrapes job listings from Wuzzuf
* Handles pagination (multiple pages)
* Extracts key job information:

  * Job Title
  * Company Name
  * City
  * Country
  * Posted Date
  * Job Link
* Cleans and structures raw HTML data
* Exports results to CSV format

---

## 🛠️ Technologies Used

* Python
* Requests
* BeautifulSoup (bs4)
* Pandas (for CSV export)

---

## 📂 Project Structure

```
wuzzuf-job-scraper/
│
├── scraper.py        # Main scraping script
├── wuzzuf_jobs.csv   # Output file
└── README.md
```

---

## ⚙️ How It Works

1. Sends HTTP requests to Wuzzuf job search pages
2. Iterates through multiple pages using pagination
3. Parses HTML using BeautifulSoup
4. Extracts job details from each listing
5. Stores results in a structured format
6. Exports data to a CSV file

---

## ▶️ How to Run

### 1. Install dependencies

```bash
pip install requests beautifulsoup4 pandas
```

### 2. Run the script

```bash
python scraper.py
```

### 3. Output

A CSV file will be generated:

```
wuzzuf_jobs.csv
```

---

## 📊 Sample Output

| Title         | Company             | City  | Country | Posted     |
| ------------- | ------------------- | ----- | ------- | ---------- |
| Data Engineer | Vertex Technologies | Cairo | Egypt   | 3 days ago |

---

## ⚠️ Notes

* The script relies on the HTML structure of the website, which may change over time.
* This project is for **educational purposes only**.

---

## 🎯 Future Improvements

* Extract job descriptions and required skills
* Store data in a database (PostgreSQL / MySQL)
* Automate scraping using scheduling tools (Airflow / Cron)
* Add data cleaning and transformation pipeline

---

## 👨‍💻 Author

Tarek Mahmoud Abdelrady
Data Engineering Student

---
