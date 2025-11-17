# 🌐 Wikipedia Web Scraper

A Python-based project that scrapes structured information from **Wikipedia pages**, such as titles, infobox content, tables, paragraphs, and links. Built using `Requests`, `BeautifulSoup`, and `Pandas`, this project is ideal for learning web scraping, data extraction, and data handling.

---

## 📌 Project Overview

This project demonstrates how to scrape data from Wikipedia using a clean and modular workflow.
The scraper can extract:

* ✔️ Page title
* ✔️ First paragraph / Summary
* ✔️ Infobox details (if available)
* ✔️ Tables (converted to Pandas DataFrames)
* ✔️ Internal links
* ✔️ References (optional)

All extracted data is displayed inside the notebook and can be exported to CSV or JSON.

---

## 🛠️ Tech Stack

### **Languages & Tools**

* Python
* Jupyter Notebook

### **Libraries Used**

* `requests` – Fetching Wikipedia page HTML
* `beautifulsoup4` – Parsing HTML content
* `pandas` – Storing & cleaning table data
* `re` – Regex for text cleaning (if used)

---

## 📂 Project Structure

```
📦 Wikipedia-Scraper
├── 📄 Wikipedia Scraping.ipynb
├── 📄 README.md
├── 📁 data
│   ├── infobox_data.csv
│   ├── table_data.csv
│   └── summary.txt
└── 📁 screenshots (optional)
```

---

## ▶️ How to Run the Project

### **1. Clone the Repository**

```bash
git clone https://github.com/your-username/wikipedia-scraper.git
cd wikipedia-scraper
```

### **2. Install Required Libraries**

```bash
pip install requests beautifulsoup4 pandas
```

### **3. Launch the Notebook**

```bash
jupyter notebook
```

Open the file: **Wikipedia Scraping.ipynb**

---

## 🧩 Features in the Notebook

### 🔹 **1. Fetch HTML Content**

* Uses `requests.get()` to fetch Wikipedia page HTML.
* Error handling for failed connections.

### 🔹 **2. Extract Page Title & Summary**

* Pulls the main heading (`<h1>` tag)
* Extracts the lead paragraph of the article

### 🔹 **3. Scrape Infobox**

* Identifies `.infobox` table
* Converts rows into structured key–value pairs
* Saves results to CSV

### 🔹 **4. Scrape HTML Tables**

* Auto-detects all `<table>` elements
* Converts tables → DataFrames
* Saves to CSV

### 🔹 **5. Extract All Internal Links**

* Collects all `/wiki/...` hyperlinks
* Filters out irrelevant or repeated links

### 🔹 **6. Save & Export**

* CSV export
* JSON export (optional)
* Display inside notebook

---

## 📊 Example Output (CSV Preview)

```
key,value
"Born", "12 January 1990"
"Occupation", "Scientist"
"Nationality", "Indian"
```

---

## 🚀 Possible Future Improvements

* Add scraping for categories
* Add summary NLP processing
* Add automated multi-page scraping
* Build a GUI or Streamlit interface

---

## 🤝 Contributing

Contributions, improvements, and suggestions are always welcome!
Feel free to open a pull request.

---

## 📜 License

This project is licensed under the **MIT License**.

---

## ⭐ Support

If this project helped you, please give it a **star ⭐ on GitHub**!
