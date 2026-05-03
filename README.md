# trends24-web-scraper-Mini-project-6

A professional Python-based web scraping system that extracts real-time trending topics from Trends24 using Playwright, processes the data, and stores it in a SQLite database.

## Features

- Real-time trend scraping from Trends24
  
- Automated browser interaction using Playwright
  
- Data cleaning and preprocessing with Pandas
  
- SQLite database integration using SQLAlchemy
  
- Structured logging system
  
- Modular and scalable project architecture
  
- Error handling and exception management
  
- Configurable scraping settings

## Project Architecture

         ```bash
         trends24-web-scraper/
         │
         ├── config/
         │   └── settings.py
         │
         ├── scraper/
         │   ├── browser.py
         │   ├── selectors.py
         │   └── trend_scraper.py
         │
         ├── data_processing/
         │   └── cleaner.py
         │
         ├── database/
         │   ├── db_connection.py
         │   └── models.py
         │
         ├── utils/
         │   └── logger.py
         │
         ├── logs/
         │   └── scraper.log
         │
         ├── main.py
         ├── check_result.py
         ├── requirements.txt
         ├── .gitignore
         └── README.md

## Technologies Used
Python

Playwright

Pandas

SQLAlchemy

SQLite

Logging Module

## Installation

### Clone Repository

          git clone https://github.com/your-username/trends24-web-scraper.git
          cd trends24-web-scraper
          
### Create Virtual Environment

          python -m venv venv
          
### Activate Virtual Environment

### Windows

          venv\Scripts\activate
          
### Linux / MacOS

          source venv/bin/activate
          
### Install Dependencies

          pip install -r requirements.txt
          
### Install Playwright Browser

          playwright install
          
### Run Project

          python main.py
          
### Database Output

The scraped data is automatically stored inside:

          trends.db

You can verify stored data using:

           python check_result.py
           
## Logging System

### Logs are stored inside:

          logs/scraper.log

### The logging system tracks:

Browser launch status

Scraping activity

Database operations

Errors and exceptions

## Configuration

All configurable settings are located in:

          config/settings.py

### Example:

          HEADLESS = False
          BASE_URL = "https://trends24.in/"
          DATABASE_URL = "sqlite:///trends.db"
          SCRAPE_LIMIT = 20
          
## Future Improvements
Multi-country trend scraping

PostgreSQL/MySQL support

Docker containerization

REST API integration

Scheduler automation (Cron Jobs)

Cloud deployment

Data visualization dashboard

## Author

### Adeel khan
