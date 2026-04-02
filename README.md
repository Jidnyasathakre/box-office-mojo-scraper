# Box Office Mojo Web Scraping 

## Overview

This project demonstrates how to scrape, clean, and analyze weekend box office data from Box Office Mojo using Python in a Jupyter Notebook.

The workflow includes:

* Fetching web pages using `requests`
* Parsing HTML using `BeautifulSoup`
* Structuring data with `pandas`
* Cleaning financial and percentage values
* Performing basic data analysis and visualization

---

## Features

* Scrapes weekend box office data for multiple years
* Extracts key fields:

  * Year
  * Date
  * Top 10 Gross
  * Overall Gross
  * Week-over-week changes (%)
* Handles missing and inconsistent values (e.g., `-`)
* Converts data into usable numeric format
* Exports cleaned dataset to CSV
* Includes basic visual analysis

---

## Technologies Used

* Python
* requests
* BeautifulSoup (bs4)
* pandas
* matplotlib

---

## Notebook Workflow

The notebook is structured into the following steps:

1. **Import Libraries**
2. **Setup Headers & URLs**
3. **Fetch Web Page Data**
4. **Parse HTML Content**
5. **Extract Table Data**
6. **Create DataFrame**
7. **Clean Data**
8. **Save Data to CSV**
9. **Basic Data Analysis & Visualization**

---

## How to Run

### 1. Install Dependencies

```bash
pip install requests beautifulsoup4 pandas matplotlib
```

### 2. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 3. Open and Run

* Open the notebook file
* Run all cells sequentially

---

## Output

The project generates a cleaned dataset:

```id="8y1e8h"
box_office_data.csv
```

Example columns:

* `year`
* `date`
* `top10_gross`
* `overall_gross`
* `top10_wow`
* `overall_wow`

---

## Sample Analysis

The notebook includes basic visualizations such as:

* Yearly total box office revenue
* Weekly revenue trends
* Average percentage change per year

---

## Notes & Limitations

* Website structure changes may break the scraper
* No advanced error logging implemented
* Data depends on availability from the source website

