# Equity_Research_Valuation_Model
This project is a Python Colab pipeline for stock valuation. It fetches historical prices and financials via yfinance and FRED, computes Beta, market risk premium, CAPM cost of equity, cost of debt and WACC, retrieves and forecasts free cash flows, runs DCF and DDM models, compares EV/EBITDA and P/E multiples, and plots results.

## 📁 Repository Structure

```text
├── Company Stock Valuation.ipynb    # Main Colab notebook with analysis pipeline
├── README.md               # Project overview and instructions
└── requirements.txt        # Python dependencies
```

## 🛠️ Requirements

* Python 3.7+
* Google Colab (online) or local Jupyter environment

Install dependencies:

```bash
pip install yfinance pandas numpy statsmodels matplotlib requests beautifulsoup4 scipy
```

Alternatively, install via `requirements.txt`:

```bash
pip install -r requirements.txt
```

## 🚀 Usage

1. **Clone** the repository:

   ```bash
   ```

git clone [https://github.com/](https://github.com/)<your-username>/EquityValuator.git
cd EquityValuator

```

2. **Open** `EquityValuator.ipynb` in Google Colab or Jupyter.

3. **Adjust parameters** (optional):
   - `ticker`: target stock symbol (default `KER.PA`).
   - `start_date` / `end_date`: historical data range.
   - Bond data: update list of `(face_value, currency, coupon_rate, maturity)` tuples.

4. **Run all cells**. The notebook will:
   - Fetch price history and financials via yfinance.
   - Scrape the French 10Y treasury yield for risk-free rate.
   - Calculate Beta, market risk premium, CAPM cost of equity, cost of debt, and WACC.
   - Retrieve and forecast free cash flows (FCF) with average-yoy, custom, and multi-stage methods.
   - Perform DCF valuations and Dividend Discount Model (DDM).
   - Compare EV/EBITDA and P/E multiples against comparables.
   - Plot valuation comparisons and metrics.

5. **Review outputs**: valuation tables, printed metrics, and saved plots.

## ⚙️ Customization

- **Target Stock**: change the `ticker` variable.
- **Date Range**: modify `start_date` / `end_date` definitions.
- **Risk-Free Source**: replace FRED URL or fallback rate.
- **Bond Portfolio**: update `detailed_bond_data` with new bonds.
- **Forecast Methods**: adjust growth rates or time horizons.

## 🤝 Contributing

1. Fork the repository
2. Create a branch (`git checkout -b feature/my-feature`)
3. Commit changes (`git commit -m "Add feature"`)
4. Push branch (`git push origin feature/my-feature`)
5. Open a Pull Request

## 📄 License

MIT License. See [LICENSE](LICENSE) for details.

---
*Harness EquityValuator to streamline and automate robust stock valuations!*

```

