# RadioEchoes Scraper

**Fast concurrent Playwright scraper** for [RadioEchoes.com](https://www.radioechoes.com) — extracts classic radio series & episodes into clean Excel/CSV with full resume support.

[![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Playwright](https://img.shields.io/badge/Playwright-Async-green?logo=playwright)](https://playwright.dev/python/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/ahmadraza-automation/radioechoes-scraper?style=social)](https://github.com/ahmadraza-automation/radioechoes-scraper)

---

### Features

| Feature | Description |
|---------|-------------|
| **Concurrent Scraping** | Scrape multiple series in parallel (configurable workers) |
| **Full Resume Support** | Stop anytime and continue later — progress is saved |
| **Clean Excel & CSV** | Structured output with Series, Episode, Genre, Date, Length, Links & File Size |
| **Headless Mode** | Run without opening browser window for maximum speed |
| **Detailed Logging** | Full run logs saved automatically |

---

### Quick Start

```bash
# 1. Clone the repo
git clone https://github.com/ahmadraza-automation/radioechoes-scraper.git
cd radioechoes-scraper

# 2. Install dependencies
pip install -r requirements.txt
playwright install chromium

# 3. Run the scraper
python main.py
```

---

### Configuration

Edit these values at the top of `main.py`:

| Setting | Default | Description |
|---------|---------|-------------|
| `HEADLESS` | `True` | `True` = faster (no browser window) |
| `CONCURRENCY` | `6` | How many series to scrape at once (4-8 recommended) |
| `TIMEOUT` | `45000` | Page load timeout in milliseconds |

---

### Output

After running, you will get:

- `output/radioechoes.xlsx` → Main data file
- `state/resume.json` → Progress tracking (for resume)
- `logs/scraper.log` → Detailed logs

---

### Sample Data

A small sample is available in [`sample_output/`](sample_output/).

---

### Author

**Ahmad Raza** — Python Automation Engineer  

- GitHub: [ahmadraza-automation](https://github.com/ahmadraza-automation)
- LinkedIn: [Ahmad Raza](https://www.linkedin.com/in/ahmad-raza-67462b413)
- Portfolio: [Live Portfolio](https://ahmadraza-automation.github.io/Ahmad-Raza-Automation-Portfolio/)
- Email: arjafri347@gmail.com

---

### Support the Project

If this project helped you or you found it useful, please consider giving it a **star**. It really helps!

```
⭐ Star this repository
```
