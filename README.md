# 📊 Automated Crypto Market Reporting System

## Overview

This project is an **Automated Crypto Market Reporting and Analysis System** built using **n8n** and **AI-based text analysis**.  
The system automatically fetches live cryptocurrency market data, processes and standardizes it, generates concise AI-driven market insights, builds professional HTML reports, and distributes them via email.

The architecture is **modular, scalable, and production-ready**, following **read-only data access** principles to ensure safety, reliability, and compliance.  

---

## System Architecture

The workflow is divided into clearly defined layers to ensure separation of concerns and easy extensibility.

---

### 🔹 Trigger Layer

- Uses a **Manual Trigger** node for development and testing
- Can be replaced with a **Schedule Trigger** for automated execution (daily, hourly, etc.) in production

---

### 🔹 Data Extraction Layer

- Fetches live cryptocurrency market data from the **CoinGecko Public API**
- No API key required for the selected endpoints
- Retrieves:
  - Current price
  - 24-hour high & low
  - Trading volume
  - All-time high & all-time low
  - Circulating and total supply
- Designed to support **multiple cryptocurrencies** with minimal changes

---

### 🔹 Data Processing Layer

- Uses **JavaScript Code nodes** to:
  - Extract required fields
  - Handle missing or undefined values
  - Format numeric data
  - Normalize the output structure
- Ensures clean, consistent, and analysis-ready data

---

### 🔹 Prompt Preparation Layer

- Constructs a structured textual prompt using processed market data
- Includes:
  - Market values
  - Timestamps
  - Contextual instructions
- Optimized for generating concise and professional AI insights

---

### 🔹 AI Analysis Layer

- Uses an **AI language model** to generate short market analysis
- Focuses on:
  - Price movement
  - Volatility
  - Liquidity
  - Risk signals
  - Overall market sentiment
- This layer performs **textual interpretation only**  
  (no numerical recalculation or data modification)

---

### 🔹 Post-Processing Layer

- Cleans AI-generated output
- Removes formatting issues or unwanted characters
- Ensures compatibility with **HTML rendering and email clients**

---

### 🔹 Report Generation Layer

- Generates a **professional HTML report** using JavaScript
- Includes structured sections:
  - Price overview
  - Volume & liquidity
  - All-time levels
  - Supply metrics
- Designed to be:
  - Email-ready
  - Visually clear
  - Easy to read for non-technical users

---

### 🔹 Distribution Layer

- Automatically sends the HTML report via:
  - Gmail
  - Outlook
  - Other SMTP-compatible email services
- Fully automated with no manual intervention required

---

## Data Flow Summary

1. Trigger initiates the workflow  
2. Market data is fetched from CoinGecko  
3. Data is cleaned and standardized  
4. A structured prompt is generated  
5. AI produces market insights  
6. Output text is post-processed  
7. An HTML report is generated  
8. The report is delivered via email  

---

## Design Principles

- Read-only data access (safe & non-invasive)
- Modular workflow architecture
- Clear separation of concerns
- Scalable and extensible design
- Production-grade automation logic

---

## Possible Extensions

- Scheduled execution (daily / hourly reports)
- Multi-cryptocurrency support
- Database or spreadsheet storage
- Slack / Telegram notifications
- Dashboard or BI tool integration
- PDF report generation

---

## Tech Stack

- **n8n** – Workflow automation
- **JavaScript** – Data processing & HTML generation
- **CoinGecko API** – Crypto market data
- **AI Language Model** – Market analysis
- **Email Services** – Report distribution

---

## Portfolio Description

> **Automated Crypto Market Reporting & Analysis System** – Designed and implemented an end-to-end automation using n8n that fetches live crypto market data, performs AI-driven analysis, generates professional HTML reports, and distributes them automatically via email. Built with modular architecture, read-only data access, and production-ready workflow design.

---

## License

MIT License – Free to use for learning, portfolio, and automation projects.
