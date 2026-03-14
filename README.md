# 📗 Beneish M‑Score Screener for the S&P 500 — **v4 (Student Edition)**
This notebook computes the **Beneish M‑Score** for S&P 500 companies to *screen* for potential earnings manipulation risk.

**NB!** To interact with this notebook (run code, make changes, or save your work), please go to `File > Save a copy in Drive` to create your own editable version. You will not be able to run code or make permanent changes to this shared version.

**What’s inside**
1. 📦 Install dependencies (Colab-friendly)
2. 📋 Pull S&P 500 constituents (from Wikipedia)
3. 🧮 Fetch financials via `yfinance` (annual ➜ quarterly fallback)
4. 🔎 Compute the 8 Beneish inputs (DSRI, GMI, AQI, SGI, DEPI, SGAI, LVGI, TATA) and the **M‑Score**
5. 🧰 Robust label matching using fuzzy search (handles "SG&A", "Selling General And Administrative", etc.)
6. 🧾 **Data lineage** columns: which exact labels were matched for each field
7. 📤 Export **CSV** and **Excel** (with red/green conditional formatting and a “Flagged” filter)
8. ⚠️ Caveats and interpretation tips

> **Reminder:** The Beneish M‑Score is a **screening tool** — **not** proof of manipulation. Always inspect filings and context.
>
## 🎯 Learning goals
By running this notebook, you will be able to:
- Explain the intuition behind each Beneish ratio
- Reproduce a systematic screen on a large universe (S&P 500)
- Interpret results with appropriate caution
- Export results for further analysis (CSV / Excel)
