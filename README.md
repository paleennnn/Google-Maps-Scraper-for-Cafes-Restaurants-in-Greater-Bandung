# 🗺️ Google Maps Scraper for Cafes & Restaurants in Greater Bandung

An automated **Python-based scraping bot** using **Selenium** to collect cafe and restaurant data from **Google Maps** across the **Greater Bandung (Bandung Raya)** area, Indonesia.  
Ideal for **business analysis**, **academic research**, and **data collection projects**.

---

## ✨ Features

### 🎯 Core Functionality
- 🔍 **Direct Google Maps Scraping** – Extracts detailed business listings
- ☕ **Multi-Category Support** – Cafes, restaurants, and coffee shops
- 🗺️ **Complete Coverage** of Bandung Raya:
  - Kota Bandung (30 kecamatan)
  - Kabupaten Bandung (31 kecamatan)
  - Kabupaten Bandung Barat (16 kecamatan)
  - Kota Cimahi (3 kecamatan)

### 📊 Data Extraction
- **Merchant Name** – Business name  
- **Address** – Full location details  
- **Phone Number** – Contact information  
- **Rating** – Google Maps rating (1–5 scale)  
- **Website** – Official website (if available)  
- **Source** – Data provenance tracking  

### 🛡️ Technical Features
- 🧠 **Smart Scrolling** with anti-stuck detection  
- 🛡️ **Anti-Bot Detection**
  - User-agent rotation  
  - WebDriver stealth injection  
- 🔄 **Automatic Deduplication**
- 📁 **Dual Output**
  - CSV (checkpoint & raw)
  - Styled Excel (.xlsx)
- 🖥️ **Interactive CLI Menu** (region & district selection)
- 📈 **Data Validation** – Filters non-Bandung area results  

---

## 🧰 Tech Stack

| Technology | Purpose |
|----------|--------|
| **Python 3** | Core programming language |
| **Selenium** | Web automation & scraping |
| **Chrome WebDriver** | Browser automation |
| **Pandas** | Data processing |
| **OpenPyXL** | Excel formatting |
| **WebDriver Manager** | Driver management |

---

## 📦 Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/paleennnn/Google-Maps-Scraper-for-Cafes-Restaurants-in-Greater-Bandung.git
cd Google-Maps-Scraper-for-Cafes-Restaurants-in-Greater-Bandung
```

### 2️⃣ Create Virtual Environment (Recommended)

**Windows**
```bash
python -m venv venv
venv\Scripts\activate
```

**Linux / macOS**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

⚠️ **Prerequisite:** Google Chrome must be installed.

---

## 🚀 Usage Guide

### ▶️ Run the Scraper
```bash
python main.py
```

### 🔄 Workflow
1. Run script → Interactive CLI appears
2. Select Region
3. Select District (kecamatan)
4. Automated process:
   - Searches Google Maps
   - Scrolls & collects merchant URLs
   - Extracts business details
   - Filters non-Bandung data
   - Removes duplicates
   - Exports CSV & Excel

### 🖥️ Example Output
```
[LOADING] Membuka Google Maps untuk: Cafe di Andir Bandung...
[SCROLL] Attempt 1: Ditemukan 15 items unik
[EXTRACTED] (1/15) Nama Cafe Pertama
[SUCCESS] Ditemukan 10 merchant
✓ File final disimpan: data_di_andir.xlsx
```

---

## 📂 Output Files

### 📊 CSV (Raw / Checkpoint)
```
data_di_[kecamatan].csv
```
- UTF-8 with BOM
- Auto checkpoint during scraping

### 📈 Excel (Formatted)
```
data_di_[kecamatan].xlsx
```

**Excel Features:**
- ✅ Auto numbering
- ✅ Colored header
- ✅ Professional borders
- ✅ Wrapped text (address)
- ✅ Frozen header row
- ✅ Center-aligned numeric columns
- ✅ Optimized column width

---

## 🎨 Project Structure
```
bandung-scraper/
├── main.py
├── requirements.txt
├── README.md
├── .gitignore
├── error.log
└── data/
    ├── data_di_andir.csv
    ├── data_di_batujajar.csv
    └── data_di_cimahi_selatan.csv
```

---

## ⚙️ Configuration & Customization

### Modify Search Categories
```python
target_types = ["Cafe", "Restoran", "Coffee Shop"]
```

### Adjust Scraping Limit
```python
results = scrape_gmaps(query, limit=30)
```

### Enable / Disable Headless Mode
```python
# options.add_argument("--headless=new")
```

---

## 🛑 Disclaimer

- This project is intended for **educational and research purposes only**.
- Scraping Google Maps may violate Google's Terms of Service.
- Use responsibly and at your own risk.

---

## 📌 Notes

- Google Maps UI may change anytime
- Excessive requests may cause temporary IP blocking
- Data accuracy depends on listing completeness
- Please respect ethical scraping practices

---

## 🐛 Troubleshooting

| Issue | Solution |
|-------|----------|
| ChromeDriver error | `pip install --upgrade webdriver-manager` |
| No results found | Check internet / increase wait time |
| Too many errors | IP blocked → wait 15 mins or use VPN |
| Stale element error | Disable headless mode for debugging |

---

## 📊 Performance Metrics

| Metric | Value |
|--------|-------|
| Avg time / district | 10–15 minutes |
| Businesses / district | 50–100 |
| Success rate | 85–90% |
| Coverage | ±80 districts |
| Data accuracy | ~95% |

---

## 👤 Author

**Febyan Valentino**  
📍 Ponorogo, Indonesia  
📚 Academic & Data Scraping Project

---

## ⭐ Support This Project

If this project helps you:

- ⭐ Star the repository
- 🍴 Fork it
- 🐛 Report issues or suggestions

---

## 📄 License

Open-source for educational purposes.  
Please use responsibly and comply with data privacy regulations.

---

**Last Updated:** January 2026  
**Compatible with Google Maps UI:** January 2026
