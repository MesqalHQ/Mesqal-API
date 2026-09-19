# ⚡ Mesqal API

<div align="center">

# Mesqal API

The data engine powering the Mesqal ecosystem.

Collecting, processing, and publishing financial market data for currencies, gold, cryptocurrencies, and more.

</div>

---

## 🌍 Overview

Mesqal API is the backend data infrastructure behind the Mesqal platform.

It continuously gathers market data, processes it into structured datasets, and publishes JSON endpoints consumed by Mesqal Web, Android, and Desktop applications.

Designed to be:

- ⚡ Fast
- 🔄 Automated
- 🌐 Serverless
- 📦 Lightweight
- 🛠 Easy to maintain

---

## ✨ Features

### 💱 Currency Data

Track exchange rates including:

- USD
- EUR
- GBP
- AED
- TRY
- and more...

### 🪙 Gold Prices

Monitor:

- Gold
- Gold Coins
- Pamp Suisse Gold Bar

### ₿ Cryptocurrency Data

Access cryptocurrency pricing and historical data.

### 📈 Historical Records

Automatically store and publish historical snapshots.

### 🔄 Scheduled Updates

Data is refreshed automatically through GitHub Actions.

### 📦 JSON Endpoints

Simple machine-readable responses for web, mobile, desktop, and third-party integrations.

### 🌍 Public Access

No authentication required for public market endpoints.

---

## 🏗 Architecture

```text
External Data Sources
          │
          ▼
GitHub Actions Workflows
          │
          ▼
Data Processing Scripts
          │
          ▼
JSON Generation
          │
          ▼
GitHub Pages
          │
          ▼
Mesqal Clients
```

---

## 📂 Repository Structure

```text
Mesqal-API/
│
├── data/
│   ├── date.json
│   └── {date}.json
│
├── .github/
│   ├── workflows/deploy-pages.yml
│   └── workflows/fetch-data.yml
│
└── README.md
```

---

## 🔗 Endpoints

Example structure:

```text
/data/dates.json
/data/{date}.json => like 2026-09-19.json
```

---

## 🔄 GitHub Actions

Mesqal API is designed to operate automatically using GitHub Actions.

Responsibilities include:

- Fetching fresh market data
- Generating JSON files
- Publishing updates
- Maintaining historical records
- Deploying to GitHub Pages

---

## 🌐 Ecosystem

Mesqal consists of multiple projects working together:

| Repository | Purpose |
|------------|----------|
| Mesqal-API | Data Collection & Processing |
| Mesqal-Web | Financial Dashboard |
| Mesqal-Android | Mobile Application |
| Mesqal-Desktop | Desktop Application |

---

## 🎯 Goals

- Reliable market data
- Open access
- Automated updates
- Historical tracking
- Lightweight infrastructure
- Easy integration

---

## 🛣️ Roadmap

- [ ] More data providers
- [ ] Better redundancy
- [ ] Historical archive expansion
- [ ] Advanced analytics
- [ ] Public documentation
- [ ] API versioning
- [ ] Developer SDKs

---

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Open a Pull Request

---

## 📄 License

MIT License

Feel free to use, modify, and distribute.

---

<div align="center">

Built with ❤️ by Amirmasoud

**Powering the Mesqal Ecosystem**

</div>
