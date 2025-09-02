# 📊 Atomberg Share-of-Voice (SoV) Agent — YouTube Prototype

This project is a prototype **AI agent** to estimate **Share of Voice (SoV)** for the keyword **“smart fan”** (and related terms) on YouTube, with a focus on **Atomberg vs. competitors** (Havells, Crompton, Orient, etc.).

The agent fetches the **top-N YouTube search results**, extracts brand mentions, estimates engagement, and computes **Results SoV**, **Engagement SoV**, and basic **sentiment analysis**.  

---

## 🚀 Features
- ✅ Fetch top-N search results for queries like `smart fan`, `BLDC fan India`, etc.  
- ✅ Compute:
  - **Results SoV** = share of results mentioning each brand.  
  - **Engagement SoV** = engagement-weighted brand share.  
  - **Sentiment** = polarity of titles/snippets.  
- ✅ Export results as **CSV report**.  
- ✅ Includes a **two-pager docx brief** with insights & recommendations for Atomberg’s marketing team.  
- ✅ Works with **YouTube Data API** (preferred) or a lightweight **HTML parse fallback** (prototype-only).  

---

## 🛠️ Tech Stack
- **Python 3.10+**
- **YouTube Data API v3** (if `YOUTUBE_API_KEY` is provided)
- **Libraries:**  
  - `google-api-python-client` (YouTube API)  
  - `requests`, `beautifulsoup4` (scraping fallback)  
  - `pandas` (data handling)  
  - `textblob` (sentiment)  
  - `python-dotenv` (API key management)  

---

## 📂 Project Structure
Atomberg_SoV_Agent/
│── main.py # CLI entry point
│── utils.py # YouTube fetch, SoV computation, sentiment
│── requirements.txt # Dependencies
│── .env.example # Example API key env file
│── README.md # This file
│── notebooks/ # Placeholder for analysis notebooks
│── two-pager/ # Contains the docx 2-pager brief
