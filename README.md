# YouTube Trending Videos – ETL Pipeline (India)

This project demonstrates a real-world ETL pipeline using Python. We extract trending video data from YouTube’s Data API, transform it into structured tabular format, and load it into a SQLite database. This pipeline is designed to mimic production data engineering workflows.

## Overview

- **Extract**: Uses YouTube Data API v3 to fetch trending videos for India (`regionCode='IN'`)
- **Transform**: Parses and cleans the JSON response, extracts relevant video info, and adds a timestamp
- **Load**: Saves the clean data into a SQLite database (`youtube_trending.db`)
- **Bonus**: Visualizes the most viewed, liked, and frequent channels in the trending list

## 🛠️ Tech Stack

- Python 3.x
- pandas
- SQLite
- Google YouTube Data API
- seaborn / matplotlib


## 🔧 Setup Instructions for API key

1. Get a free API key from Google Cloud Console:
   - Enable **YouTube Data API v3**
   - Create API credentials
2. Paste your API key into the script like:
   ```python
   YOUTUBE_API_KEY = "your_key_here"
