# NinjaTrader Historical Data Exporter

A NinjaTrader 8 strategy that exports historical price data and EMA indicators to CSV format.

## Files

- **[ninjascripts/HistoricalData.cs](ninjascripts/HistoricalData.cs)** - NinjaTrader strategy for data export
- **[data/HistoricalData.csv](data/HistoricalData.csv)** - Sample exported historical data

## Quick Start

1. Copy `HistoricalData.cs` to your NinjaTrader scripts folder:
   ```
   Documents\NinjaTrader 8\bin\Custom\Strategies\
   ```

2. Compile in NinjaTrader (F5)

3. Apply strategy to any chart to export data

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
