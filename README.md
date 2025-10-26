# 📈 Stock Trading Analysis Tool

A comprehensive Jupyter notebook for analyzing your stock trading decisions using moving averages (50-DMA and 200-DMA) to evaluate both buy and sell timing.

## 🎯 Features

- **Buy Decision Analysis**: Evaluate your entry points against market conditions
- **Sell Timing Analysis**: Determine if you sold too early or at the right time
- **Moving Average Analysis**: Compare your trades against 50-day and 200-day moving averages
- **Financial Year Breakdown**: Performance analysis by Indian FY (April-March)
- **Opportunity Cost Calculation**: See what you missed or saved by your decisions
- **Multiple File Support**: Upload and combine multiple tax P&L reports
- **Comprehensive Metrics**: Success rates, average profit, best/worst periods

## 📋 Requirements

- Python 3.8+
- Google Colab (recommended) or Jupyter Notebook
- Required Python packages (auto-installed in notebook):
  - yfinance
  - pandas
  - openpyxl

## 🚀 Quick Start

### Using Google Colab (Recommended)

1. **Open the notebook in Google Colab:**
   - Go to [Google Colab](https://colab.research.google.com/)
   - Click `File` → `Open notebook` → `GitHub` tab
   - Enter your repository URL or upload the notebook directly

2. **Upload your Tax P&L file(s):**
   - The notebook will prompt you to enter how many files to upload
   - Upload your Zerodha Tax P&L Excel files (typically named `taxpnl-*.xlsx`)

3. **Run all cells:**
   - Click `Runtime` → `Run all`
   - Wait for the analysis to complete (may take a few minutes)

4. **Download results:**
   - The analyzed results will be automatically saved as CSV
   - Review the summary analytics in the notebook

### Using Local Jupyter Notebook

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/stock-analysis.git
cd stock-analysis

# Install dependencies
pip install -r requirements.txt

# Start Jupyter
jupyter notebook Stock_Analysis_Updated.ipynb
```

## 📊 Input File Format

The notebook expects Zerodha Tax P&L Excel files with the following structure:
- **Symbol**: Stock ticker symbol
- **Entry Date**: Buy date
- **Exit Date**: Sell date
- **Quantity**: Number of shares
- **Buy Value**: Total purchase price
- **Sell Value**: Total selling price
- **Profit**: Actual profit/loss (will be renamed to "Actualised Profit")

## 📈 Output

The analysis provides:

### 1. **Buy Analysis**
- Market conditions at entry (vs 50-DMA & 200-DMA)
- Buy verdict (Good call/Bad call based on profitability)

### 2. **Sell Analysis**
- Market conditions at exit
- Sell verdict (Good call if price fell, Wrong early sell if price rose)
- Current price comparison

### 3. **Financial Metrics**
- Actualised Profit: Your actual gain/loss
- Opportunity Cost/Gain: What you could have made by holding

### 4. **Summary Analytics**
- Performance breakdown by financial year
- Overall success rates
- Best and worst performing periods
- Average profit per trade

## 📁 Repository Structure

```
stock-analysis/
├── Stock_Analysis_Updated.ipynb    # Main analysis notebook
├── README.md                        # This file
├── requirements.txt                 # Python dependencies
├── .gitignore                       # Git ignore rules
├── LICENSE                          # License file
└── sample_output/                   # Sample output files (optional)
    └── analyzed_trades_sample.csv
```

## 🔒 Privacy & Security

- **Never commit sensitive data**: Your actual trading data should NOT be pushed to GitHub
- The `.gitignore` file is configured to exclude:
  - CSV files with trading data
  - Excel files (*.xlsx)
  - Personal data files
  - Colab auth files

## 🛠️ Customization

### Modify Moving Average Periods
In the `calculate_moving_averages` function, change:
```python
data['50_DMA'] = data['Close'].rolling(window=50).mean()
data['200_DMA'] = data['Close'].rolling(window=200).mean()
```

### Change Stock Data Source
Currently uses Yahoo Finance (yfinance). Can be modified to use other data providers.

## 📝 Future Enhancements (TODO)

- [ ] Fix stock split inaccuracies (detect and adjust historical prices)
- [ ] Handle stock name changes and "-" issues (create mapping)
- [ ] Add news analysis integration
- [ ] Statistical pattern analysis with respect to DMA
- [ ] LLM integration for decision analysis
- [ ] Context tracking (market falls, stop-loss triggers)
- [ ] Sector/industry analysis
- [ ] Compare against index performance (Nifty/Sensex)
- [ ] Interactive visualizations
- [ ] Web dashboard version

## 🤝 Contributing

This is a private repository. If you'd like to contribute:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

This tool is for educational and analytical purposes only. Past performance does not guarantee future results. Always consult with a qualified financial advisor before making investment decisions.

## 🙏 Acknowledgments

- Yahoo Finance API for historical stock data
- Zerodha for trading platform and tax reports
- The open-source community for various Python libraries

## 📧 Support

For issues, questions, or suggestions, please open an issue in the GitHub repository.

---

**Happy Trading! 📊💰**
