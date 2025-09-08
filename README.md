# usds-ecfr # USDS eCFR Insights

This repository contains my submission for the **USDS Engineering Take-Home Assessment**.  
The goal of this project is to ingest **federal regulations** data from the [eCFR API](https://www.ecfr.gov/developers/documentation/api/v1), store it server-side, provide APIs for retrieving and analyzing it, and expose a simple **frontend UI** for actionable insights.

---

## Features

- **Data ingestion** from the official eCFR API
  - Titles, versions, structures, and full XML text
- **Server-side storage** in SQLite with SQLAlchemy
- **RESTful API endpoints** (FastAPI) to:
  - Ingest snapshots for one or more Titles by date
  - Retrieve latest per-title metrics
  - View historical metrics over time
  - Aggregate metrics by agency (if mapping is available)
- **Analysis metrics**
  - Word count per Title
  - Section count per Title
  - SHA-256 checksum per snapshot
  - Historical word-count tracking
  - **Custom metric:** *Readability Index* (approximate Flesch-Kincaid grade level)
- **UI dashboard** (HTML + Chart.js)
  - Trigger ingestion
  - Explore agency and title-level metrics
  - Visualize historical trends

---

## Quickstart

### 1. Clone and install dependencies
```bash
git clone https://github.com/ahier/usds-ecfr.git
cd usds-ecfr
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
