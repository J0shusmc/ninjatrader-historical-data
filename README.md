# NinjaTrader Historical Data Exporter

A NinjaTrader 8 strategy that exports historical price data and EMA indicators to CSV format.

## Files

- **[ninjascripts/HistoricalData.cs](ninjascripts/HistoricalData.cs)** - NinjaTrader strategy for data export
- **[data/HistoricalData.csv](data/HistoricalData.csv)** - Sample exported historical data

## Installation & Setup

### IMPORTANT: Strategy Name Requirement
You **MUST** create a new strategy named **"HistoricalData"** in NinjaTrader. The strategy will not compile if you use any other name without making the necessary changes to the code.

### Steps:

1. In NinjaTrader 8, go to **Tools → New NinjaScript → Strategy**

2. Name the strategy **exactly**: `HistoricalData`

3. Click **OK** to create the strategy template

4. Open the newly created strategy file and **replace all code** with the contents of `HistoricalData.cs` from this repository

5. Compile the script (F5)

6. Apply the strategy to any chart to begin exporting data

## Output Format

```csv
DateTime,Open,High,Low,Close,EMA21,EMA75,EMA150
01/15/2025 09:00:00,4850.25,4852.50,4848.00,4851.75,4850.12,4849.88,4848.50
```

## Features

- OHLC price data export on bar close
- EMA 21, 75, and 150 indicators
- Configurable output path
- Error handling and data validation

## License

MIT
