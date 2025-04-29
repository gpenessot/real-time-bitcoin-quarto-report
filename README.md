# 📊 Real-Time Bitcoin Reporting with Quarto & Python

This project demonstrates how to build a fully automated, real-time report using **Quarto**, **Python**, and **Plotly**, with live data fetched from the **Coinbase API**.

You’ll generate a beautiful HTML report showing:
- A candlestick chart of the last 10 minutes of BTC/USD prices,
- Volume traded,
- A quick interpretation of market dynamics.

---

## 🚀 Preview

👉 [Live Report Demo](https://gpenessot.github.io/real-time-bitcoin-quarto-report/)  
*(Optional if deployed via GitHub Pages)*

---

## 📦 Technologies Used

- [Quarto](https://quarto.org/) – report engine
- [Python 3](https://www.python.org/)
- [Pandas](https://pandas.pydata.org/) – data manipulation
- [Plotly](https://plotly.com/python/) – interactive charts
- [Coinbase API](https://docs.cloud.coinbase.com/exchange/docs/rest-api) – data source

---

## 📁 Project Structure

```
├── report.qmd             # Quarto markdown file (main logic)
├── requirements.txt       # Python dependencies
└── docs/                  # Output folder for GitHub Pages (optional)
```

---

## 🔧 Installation

Clone the repo and set up your environment:

```bash
git clone git@github.com:gpenessot/real-time-bitcoin-quarto-report.git
cd your-repo-name
python -m venv venv
source venv/bin/activate  # or .\venv\Scripts\activate on Windows
pip install -r requirements.txt
```

---

## ▶️ Render the Report

```bash
quarto render report.qmd
```

The report will be generated as `report.html` (or in the `docs/` folder if configured for GitHub Pages).

---

## 🌐 Deploy to GitHub Pages (Optional)

1. In `_quarto.yml`, add:
```yaml
output-dir: docs
```

2. In GitHub repo settings, enable Pages on the `main` branch under `/docs`.

3. Push to GitHub and your report will be live!

---

## 🧪 Example Output

- Candlestick chart over the last 10 minutes
- Volume bars
- Dynamic textual analysis (variation, amplitude, volume)
- Fully interactive with Plotly

---

## 💡 Future Improvements

- Add technical indicators (RSI, MACD)
- Fetch historical data over longer periods
- Schedule automatic rebuilds (e.g. with GitHub Actions or cron)

---

## 📣 Author

Gaël Penessot – [@gaelpenessot](https://www.linkedin.com/in/gael-penessot/)  
Content creator and data trainer – Python, SQL, Git & Modern Reporting

---

## 📬 Stay Informed

📩 Subscribe to the [newsletter](https://datagyver.substack.com/subscribe) to get more tutorials like this and updates about the upcoming **Quarto training**.
