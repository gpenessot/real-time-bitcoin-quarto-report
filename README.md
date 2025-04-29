# 📊 Real-Time Bitcoin Report with Quarto

This project demonstrates how to automate the creation of a real-time, interactive Bitcoin price report using:

- 🐍 **Python** (with [Plotly](https://plotly.com/), `requests`, `pandas`)
- 📄 **Quarto** for document generation
- 🌐 **Coinbase API** for real-time data
- 🚀 **GitHub Pages** for deployment
- ⚡ **[uv](https://github.com/astral-sh/uv)** as the Python package manager

---

## 🔧 Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/gpenessot/real-time-bitcoin-quarto-report.git
cd real-time-bitcoin-quarto-report
```

### 2. Create and activate a virtual environment using `uv`

```bash
uv venv
. .venv/Scripts/activate  # On Windows
# Or:
source .venv/bin/activate  # On Unix/Mac
```

### 3. Install dependencies from `pyproject.toml`

```bash
uv pip install -e .
```

> This installs all necessary packages including `pandas`, `plotly`, `requests`, and `jupyter` if defined in your `pyproject.toml`.

### 4. Set the Python path for Quarto (temporary in current shell)

```powershell
$env:QUARTO_PYTHON = "$PWD\.venv\Scripts\python.exe"
```

On Unix/Mac:
```bash
export QUARTO_PYTHON="$PWD/.venv/bin/python"
```

---

## 🚀 Render the Quarto Report

```bash
quarto render
```

This will generate the HTML report inside the `/docs` folder.

---

## 🌍 Deploy on GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings > Pages**
3. Select branch `main` and folder `/docs`
4. Click **Save**

For example, my report will be available at: [https://gpenessot.github.io/real-time-bitcoin-quarto-report/](https://gpenessot.github.io/real-time-bitcoin-quarto-report/)

---

## 📁 Project Structure

```
.
├── .venv/                  # Virtual environment (not pushed)
├── report.qmd              # Main Quarto report
├── pyproject.toml          # Project dependencies
├── _quarto.yml             # Quarto configuration
├── docs/                   # Generated HTML for GitHub Pages
└── README.md
```

---

## 🧠 Credits & Acknowledgements

Created by [@gaelpenessot](https://www.linkedin.com/in/gael-penessot/).

Data provided by [Coinbase API](https://docs.cloud.coinbase.com/exchange/docs/rest-api)

---

## 📬 Stay Updated

📩 Subscribe to the [newsletter](https://datagyver.substack.com/subscribe) to get more tutorials like this and updates about the upcoming **Quarto training**.
