# 📈 Yell.com Business Lead Extractor

> **A scalable web scraping pipeline for automated business data collection and structured lead generation.**

---

## 📋 Overview
This project is a multi-stage data extraction tool designed to scrape business information from **Yell.com**. It utilizes **Selenium** for browser automation and is structured across **Jupyter Notebooks** to allow for iterative data processing and cleaning. The system is capable of handling large-scale extractions by iterating through town lists and business categories.

## 🚀 Key Features
* **Multi-Stage Pipeline:** Uses separate scripts for link harvesting (`first_script`) and detailed data extraction (`second_script`).
* **Town-Based Iteration:** Dynamically scrapes data based on a provided list of towns (`towns.csv`).
* **Structured Output:** Automatically saves and organizes data into CSV format for easy integration with Excel, SQL, or BI tools.
* **Dynamic Content Management:** Optimized to handle Yell.com’s pagination and dynamic elements using Selenium.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Workflow:** Jupyter Notebooks (.ipynb)
* **Automation:** Selenium WebDriver
* **Data Format:** CSV (Comma Separated Values)

## 📂 Repository Structure
* `first_script.ipynb`: Initial link harvester to collect business profile URLs.
* `second_script.ipynb`: Detailed scraper to extract phone numbers, addresses, and ratings.
* `towns.csv`: Input file containing target locations.
* `bussinessLinks.csv`: Intermediate storage for profile URLs.
* `sampleData.csv`: Example of the final structured output.

## ⚙️ How to Use
1. **Setup:** Install Selenium and ensure your WebDriver (ChromeDriver) is in your PATH.
2. **Input:** Update `towns.csv` with your target locations.
3. **Execution:** Run the notebooks in order to generate the lead database.

---
**Disclaimer:** This project is for educational and research purposes. Please respect Yell.com's Terms of Service and scraping policies.
