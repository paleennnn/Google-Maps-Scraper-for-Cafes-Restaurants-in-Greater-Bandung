📍 Google Maps Scraper for Cafes & Restaurants in Greater Bandung

An automated Google Maps scraping bot built using Python & Selenium to collect data from cafes, restaurants, and coffee shops across the Greater Bandung (Bandung Raya) area, Indonesia.

This project provides structured, clean, and formatted data exports in both CSV and Excel, suitable for business analysis, academic research, and data collection tasks.

✨ Features

🔍 Scrapes business listings directly from Google Maps

☕ Supports multiple categories:

Cafe

Restaurant

Coffee Shop

🗺️ Coverage Area (Bandung Raya):

Kota Bandung

Kabupaten Bandung

Kabupaten Bandung Barat

Kota Cimahi

📊 Extracted Data:

Merchant Name

Address

Phone Number

Rating

Website (if available)

Data Source

🧠 Smart scrolling & anti-stale element handling

🛡️ Basic anti-bot detection techniques

User-agent rotation

Smart delay

WebDriver stealth injection

🔄 Automatic data deduplication

📁 Output formats:

CSV (checkpoint & raw data)

Styled Excel (.xlsx)

🖥️ Interactive CLI menu for region & district selection

🧰 Tech Stack

Python 3

Selenium

Chrome WebDriver

Pandas

OpenPyXL

WebDriver Manager

📦 Installation
1. Clone the Repository
git clone https://github.com/yourusername/google-maps-bandung-scraper.git
cd google-maps-bandung-scraper

2. Create Virtual Environment (Recommended)
python -m venv venv
source venv/bin/activate  # Linux / Mac
venv\Scripts\activate     # Windows

3. Install Dependencies
pip install -r requirements.txt


⚠️ Google Chrome must be installed on your system.

🚀 Usage

Run the scraper:

python scraper.py

Workflow:

Select region (Kota / Kabupaten)

Select district (kecamatan)

The bot will:

Search Google Maps

Scroll & collect merchant URLs

Extract detailed business information

Filter non-Bandung area results

Remove duplicate entries

Export CSV & formatted Excel files

📂 Output Files

CSV (Checkpoint / Raw Data)

data_di_<kecamatan>.csv


Formatted Excel File

data_di_<kecamatan>.xlsx

Excel Features:

Auto numbering

Colored headers

Borders for all cells

Wrapped text for long addresses

Frozen header row

🛑 Disclaimer

This project is intended for educational and research purposes only.

Scraping Google Maps may violate Google’s Terms of Service.
Use responsibly and at your own risk.

📌 Notes

Google Maps UI structure may change at any time

Accuracy depends on page layout and availability of data

Excessive usage may result in temporary IP blocking

👤 Author

Febyan Valentino
📍 Bandung, Indonesia
📚 Academic & Data Scraping Project

⭐ Support

If this project helps you:

⭐ Star the repository

🍴 Fork it

🧠 Improve or refactor the code