# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2025-10-26

### Added
- Initial release of Stock Trading Analysis Tool
- Support for Zerodha Tax P&L Excel files
- Buy decision analysis with market conditions (50-DMA & 200-DMA)
- Sell timing analysis with opportunity cost calculation
- Multiple file upload support
- Financial year breakdown (Indian FY: April-March)
- Comprehensive summary analytics:
  - Buy success rate
  - Sell timing success rate
  - Average profit per trade
  - Best/worst performing financial years
- Actualised profit tracking (renamed from "Profit")
- Buy verdict based on profitability
- Sell verdict based on price movement after sale
- Current price tracking vs historical sell prices
- CSV export functionality
- Google Colab compatibility

### Features
- Automatic duplicate removal across multiple files
- 5-year historical data download via Yahoo Finance
- Moving average calculations (50-DMA, 200-DMA)
- Error handling for missing data
- Date format validation
- Numeric column conversion with error handling

### Documentation
- Comprehensive README with usage instructions
- Setup guide for GitHub repository
- Requirements file for dependencies
- MIT License
- .gitignore configured for sensitive data protection

### TODO (Future Enhancements)
- Stock split detection and adjustment
- Stock name change handling
- News integration for context
- Statistical pattern analysis
- LLM integration for decision insights
- Sector/industry analysis
- Index performance comparison (Nifty/Sensex)
- Interactive visualizations
- Web dashboard version

## [Unreleased]

### Planned
- Data visualization charts
- Portfolio performance tracking
- Risk metrics (Sharpe ratio, max drawdown)
- Export to multiple formats (Excel, PDF)
- Automated email reports
- Mobile-friendly version

---

## Version History Format

### [Version] - YYYY-MM-DD

#### Added
- New features

#### Changed
- Changes in existing functionality

#### Deprecated
- Soon-to-be removed features

#### Removed
- Removed features

#### Fixed
- Bug fixes

#### Security
- Security patches
