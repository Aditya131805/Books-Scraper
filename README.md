# 📚 Books Scraper

A Python-based web scraper that extracts book data from **BooksToScrape.com** and saves it into **Excel (.xlsx)** and **CSV (.csv)** formats.

---

## 🚀 Features

* Scrapes multiple pages automatically
* Extracts:

  * Title
  * Price (£)
  * Availability
  * Rating (1–5)
* Retry mechanism for failed requests
* Batch scraping with cooldown
* Saves data in:

  * Excel (formatted)
  * CSV (raw)
* Clean and structured output

---

## 🛠️ Tech Stack

* Python 3
* requests
* beautifulsoup4
* openpyxl

---

## 📂 Project Structure

```
books-scraper/
│── main.py
│── requirements.txt
│── README.md
│── Scraped_Books_Data.xlsx   (generated)
│── Scraped_Books_Data.csv    (generated)
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository

```
git clone https://github.com/Aditya131805/Books-Scraper.git
cd Books-Scraper
```

---

### 2️⃣ Create Virtual Environment (Recommended)

```
python -m venv venv
```

Activate it:

* Windows:

```
venv\Scripts\activate
```

* Mac/Linux:

```
source venv/bin/activate
```

---

### 3️⃣ Install Requirements

```
pip install -r requirements.txt
```

---

## ▶️ Run the Scraper

```
python main.py
```

---

## 📊 Output Files

### 📘 Excel File

* `Scraped_Books_Data.xlsx`
* Styled headers
* Proper column widths

### 📄 CSV File

* `Scraped_Books_Data.csv`
* Lightweight format for analysis

---

## 🔄 How It Works

1. Sends HTTP requests to each page
2. Parses HTML using BeautifulSoup
3. Extracts book details
4. Stores data in batches
5. Saves progress after each batch
6. Stops when no more pages are found

---

## ⚠️ Important Notes

* Close Excel file before running (to avoid permission error)
* Uses delay to prevent blocking
* For educational purposes only

---

## 📈 Future Improvements

* Add progress bar (tqdm)
* Logging system
* Database storage (MySQL/MongoDB)
* Filters (price, rating)
* Web UI (Flask/React)

---

## 📜 License

This project is for educational purposes.

---

## 🙌 Acknowledgment

Data source: https://books.toscrape.com/
