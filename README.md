
# 📰 Haryana News Scraper

This repository contains a Python-based web scraper that automatically collects and processes the latest news articles from the official **Haryana government website**. The project is built using `requests`, `BeautifulSoup`, and `pandas` for HTML parsing, data cleaning, and storage.

## 📌 Features

* ✅ Automatically fetches latest news articles.
* ✅ Extracts titles, publication dates, and links.
* ✅ Converts relative paths to absolute URLs.
* ✅ Cleans and filters the data to remove duplicates or empty entries.
* ✅ Saves the structured data into a CSV file for easy integration and analysis.

## 🛠️ Technologies Used

* Python 3.x
* [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) - HTML parsing
* `requests` - for HTTP requests
* `pandas` - data manipulation and CSV output
* `datetime` - timestamping output

## 📂 File Structure

```
.
├── hr scrapper.ipynb     # Main Jupyter Notebook with full scraping script
├── output.csv            # Generated CSV file with cleaned news articles (example)
└── README.md             # Project documentation
```

## ⚙️ How It Works

1. **Send Request:** Accesses the Haryana government’s news page using `requests`.
2. **Parse HTML:** Uses BeautifulSoup to extract relevant news content.
3. **Filter & Clean:** Removes redundant HTML elements like `<script>`, `<style>`, and empty tags.
4. **Format Data:** Formats the article data (title, date, link) into a clean DataFrame.
5. **Export:** Saves the final output into a timestamped CSV file.

## 🚀 How to Run

1. Clone this repository:

```bash
git clone https://github.com/yourusername/haryana-news-scraper.git
cd haryana-news-scraper
```

2. Create a virtual environment (optional but recommended):

```bash
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Run the notebook:

* Open `hr scrapper.ipynb` in Jupyter Notebook or JupyterLab.
* Run all cells to generate the latest scraped data.

## 📈 Example Output

| Date       | Title                           | Link         |
| ---------- | ------------------------------- | ------------ |
| 2025-07-01 | CM inaugurates new projects...  | https\://... |
| 2025-06-30 | Haryana Govt releases budget... | https\://... |

