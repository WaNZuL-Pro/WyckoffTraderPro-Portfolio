````
# WyckoffTraderPro

## Cloud Engineering & Trading Automation Portfolio

WyckoffTraderPro is a personal cloud-based trading-engineering project designed to process market data, detect trading opportunities, generate trading signals and support paper-trading analysis.

The project combines cloud operations, serverless processing, database management, API integration, monitoring, troubleshooting and cost optimisation.

> The main source code and sensitive configuration are kept in a separate private repository.

---

## Project Overview

WyckoffTraderPro is designed around a controlled trading-engineering workflow:

```text
Market Data API
      ↓
Scheduled Cloud Functions
      ↓
Cloud Firestore
      ↓
Recent Candle Cache
      ↓
Structure / Setup Analysis
      ↓
Decision Engine
      ↓
Trading Signals
      ↓
Paper Trading
      ↓
Order Synchronisation
      ↓
Reports / Telegram Notifications
````

The project focuses on building a reliable and explainable process rather than relying on a single trading script.


## Main Objectives

* Process market data efficiently

* Detect market structure and trading setups

* Generate and track trading signals

* Support paper-trading workflows

* Synchronise order and trade status

* Investigate runtime and operational errors

* Monitor system behaviour through logs and notifications

* Control cloud usage and API costs

* Support backtesting and shadow-mode analysis
  
  

## Technology Stack

### Programming

* JavaScript

* Node.js

* Python for selected analysis and data-processing tasks

### Cloud & Infrastructure

* Google Cloud Functions

* Cloud Run runtime

* Cloud Firestore

* Cloud Scheduler

* Cloud Logging

* Firebase ecosystem

### Integration

* Market-data API

* Trading / paper-trading API

* Telegram Bot API

### Development & Analysis

* Visual Studio Code

* Git and GitHub

* CSV / JSON data processing

* Backtesting

* Shadow-mode analysis

* Runtime log investigation


  
## Engineering Challenges

### 1. Signal Consistency

Investigated signal flow between live signals and paper-trading signals, including duplicate-signal handling and missed signal scenarios.

### 2. Weak or Rejected Setups

Reviewed setup confirmation, risk-reward requirements and confidence levels to improve signal quality.

### 3. Cloud Runtime Errors

Investigated serverless runtime errors, function exports/imports and errors related to missing or incorrectly referenced functions.

### 4. Order Synchronisation

Reviewed polling, order-status updates, terminal states and manual-close detection.

### 5. Telegram Notification Problems

Investigated HTTP errors and message-length limitations affecting trading notifications.

### 6. API and Cloud Cost Pressure

Applied incremental fetching, batching, caching, bounded retries and targeted database queries to reduce unnecessary usage.


## Cost Optimisation Practices

The project applies several cost-conscious engineering practices:

* Incremental market-data retrieval

* Historical backfill in controlled batches

* Multi-symbol and batch processing

* Rate limiting

* Handling of HTTP 429 responses

* Bounded retry and exponential backoff

* Recent-candle tail caching

* Deterministic candle identifiers

* Batched Firestore writes

* Targeted queries for active and due trades

* Terminal-state filtering

* Scheduled polling controls

* Housekeeping and retention practices

* Budget monitoring and cost review

  

## Monitoring & Troubleshooting

Operational investigation includes:

* Cloud runtime logs

* Function execution errors

* Scheduler and timeout issues

* Database state inconsistencies

* Duplicate signal diagnostics

* Order-status mismatches

* Telegram delivery failures

* Data-processing and synchronisation issues

The project aims to make system behaviour traceable through logs, diagnostic statuses and operational records.



## Portfolio Evidence

The portfolio will include selected screenshots and documentation covering:

* Cloud deployment

* Runtime logs

* Firestore records

* Trading signal flow

* Telegram notifications

* System architecture

* Troubleshooting examples

* Cost optimisation practices

  

## Repository Structure

The public portfolio repository contains documentation and selected project evidence.

The main application source code is maintained separately in a private repository.

```
WyckoffTraderPro-Portfolio/
│
├── README.md
├── docs/
├── screenshots/
└── diagrams/
```

## Security Note

The following information must not be published:

* API keys

* Trading account credentials

* Telegram bot tokens

* Firebase service-account files

* Private keys

* `.env` files

* Private database exports

* Sensitive personal or account information

  
## Project Status

This portfolio is being developed progressively as the WyckoffTraderPro project evolves.

Future improvements may include:

* More detailed architecture diagrams

* Additional screenshots

* Public-safe code examples

* Testing documentation

* Deployment documentation

* Troubleshooting case studies

* Project demonstration materials
  

## Disclaimer

This is a personal engineering and trading-automation project.

Any trading objectives, strategy results or backtesting figures are provided for engineering and analysis context only. They are not financial advice or a guarantee of future trading performance.

````
