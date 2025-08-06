# 💼 JobMatch - AI-Powered LinkedIn Job Scraper with n8n

JobMatch is an AI-powered automation built using [n8n](https://n8n.io/) that automatically scrapes job listings from LinkedIn via RSS, processes and cleans the data using AI, and exports the final results to a Google Sheet — making job tracking, filtering, and organization effortless.

---

## 📌 Features

- 🔄 **Automated Job Scraping** – Fetches latest job postings from LinkedIn using RSS feeds.
- 🧠 **AI Integration** – Uses OpenAI (or similar models) for semantic filtering, job categorization, or scoring.
- ✍️ **Data Cleaning** – Automatically parses and structures job data (title, company, location, etc.).
- 📊 **Google Sheets Export** – Appends relevant job data into a structured Google Sheet in real-time.
- 📅 **Manual or Scheduled Execution** – Run manually or schedule it on a recurring basis.

---

## 📷 Workflow Overview

![Workflow Screenshot](./assets/workflow-ui.png)

---

## 🛠️ Tech Stack

| Tool         | Purpose                             |
|--------------|-------------------------------------|
| [n8n](https://n8n.io/)         | No-code automation and workflow orchestration |
| RSS Feed Node | Fetches job listings from LinkedIn |
| HTTP Node     | Performs external web/API requests |
| OpenAI Node / AI Parser | Applies AI-based filtering or scoring |
| Google Sheets Node | Writes final data into spreadsheet |

---

## 🚀 How It Works

1. **Trigger**: Workflow starts manually or on a schedule.
2. **RSS Read**: Fetches job listings from LinkedIn RSS feed.
3. **Limit Node**: Restricts to latest X results to avoid duplicates.
4. **HTTP Request**: Optional API or web scraping logic.
5. **AI (LLM) Parsing**: Processes job descriptions (e.g., scoring, filtering).
6. **Field Editing**: Cleans and structures the output.
7. **Google Sheets Integration**: Appends or updates job records.

---

## 🧩 Setup Instructions

> 💡 This project assumes you're familiar with [n8n](https://docs.n8n.io/getting-started/).

### 1. Clone This Repository

```bash
git clone https://github.com/yourusername/JobMatch.git
cd JobMatch
