# Weather Forecast Report Generator

An automated Python pipeline that fetches 3-day weather forecast data 
from the NAM (North American Mesoscale) numerical weather model, 
generates a formatted PDF report, and delivers it by email.

Built as part of a broader portfolio combining atmospheric data science 
with numerical weather model tools.

---

## Features
- Fetches real NAM model output for any lat/lon location
- Parses forecast variables (temperature, precipitation, wind speed, UV Index)
- Auto-generates a clean PDF weather report
- Sends the report to one recipient or a team email address automatically

---

## Requirements
- Python 3.10+
- See requirements.txt for full package list

---

## Setup

1. Clone this repository
   git clone https://github.com/tian667-op/3-day-weather-forecast-report.git

2. Install dependencies
   pip install -r requirements.txt

3. Copy .env.example to .env and fill in your credentials
   Mac / Linux / Git Bash:
   cp .env.example .env

   Windows Command Prompt:
   copy .env.example .env

   Then open the .env file and replace the placeholder 
   values with your own credentials.

4. Open the notebook and set your location in the 
   LOCATION SETTINGS cell (see Configuration below)

---

## Configuration

| Variable         | Description                        |
|------------------|------------------------------------|
| LATITUDE         | Decimal latitude of your location  |
| LONGITUDE        | Decimal longitude of your location |
| LOC_NAME         | Label used in the PDF report       |
| EMAIL_ADDRESS    | Your sender email address          |
| EMAIL_PASSWORD   | Your email app password            |
| RECIPIENTS       | Comma-separated recipient emails   |

Find your coordinates at https://www.latlong.net

---

## Data Source
NAM (North American Mesoscale Model) — NOAA's operational regional 
weather forecast model, updated 4 times daily at 6-hour intervals.
More info: https://www.ncei.noaa.gov/products/weather-climate-models/north-american-mesoscale

---

## Author
Qi Tian
GitHub: github.com/tian667-op
---

## License
MIT License — free to use and modify with attribution.
