# WTT_Waverider

A comprehensive Pine Script trading indicator for TradingView with EMA-based signals, RSI momentum analysis, and visual trend tracking.

## Features

### Core Indicators
- **EMA System**: 21-period, 50-period, and middle MA (average of both)
- **Dynamic Price Coloring**: Teal above all EMAs, maroon below all EMAs, white in between
- **RSI Momentum Analysis**: Overbought/oversold dots with extreme price highlighting

### Signal System
- **Entry Signals**: Triangle markers for long/short positions
- **Volume Filter**: Unusually high volume requirement
- **RSI Filter**: Oversold for longs, overbought for shorts
- **First Occurrence Only**: Signals show only on initial crossover

### Visual Tracking
- **Diamond Markers**: Maroon diamonds for higher highs (exit long), teal diamonds for lower lows (exit short)
- **RSI Dots**: Red/green for regular conditions, orange for extreme price points
- **Heads Up Display**: Real-time monitoring table with performance statistics

### Alert System
- **Entry Alerts**: Long/Short signal notifications with price
- **Exit Alerts**: Diamond marker notifications with exit instructions
- **RSI Alerts**: All dot types (regular and extreme conditions)

### Performance Tracking
- **Win Rate Statistics**: Long and short performance tracking
- **ATR Trend Analysis**: Rising/Falling/Sideways volatility assessment
- **Current Signal Display**: Active position monitoring

## Files

- `WTT_Syzygy_Waverider_R5.6.pine` - Main indicator script (Pine Script v5)
- `trading_rules.txt` - Comprehensive trading rules and guidelines

## Installation

1. Copy the `WTT_Syzygy_Waverider_R5.6.pine` code
2. Open TradingView and go to Pine Editor
3. Paste the code and click "Add to Chart"
4. Configure parameters as needed

## Trading Rules

### Entry Rules
- **LONG**: Green triangle when price above all EMAs + (Volume OR RSI oversold)
- **SHORT**: Red triangle when price below all EMAs + (Volume OR RSI overbought)

### Exit Rules
- **LONG Exits**: Green dot after orange dot, green dot after green dot, or teal diamond
- **SHORT Exits**: Red dot after orange dot, red dot after red dot, or maroon diamond

### Risk Management
- Use stop loss at entry price
- Take profit at 2:1 risk/reward ratio
- Maximum 2% of account per trade
- Monitor HUD table for market conditions

## Version History

### R5.x Series (Current)
- R5.10: Changed alert conditions to plain alerts
- R5.9: Added lower low X markers after long signals
- R5.8: Added higher high X markers after short signals
- R5.7: Added alert conditions for signals with closing price
- R5.6: Changed "ATR Trend" to "Trend" in table
- R5.5: Made table text slightly bigger
- R5.4: Made current signal persist until next signal fires
- R5.3: Made table text smaller and added current signal row
- R5.2: Changed extreme dots to egg yolk color and smaller size
- R5.1: Made yellow extreme dots bigger
- R5.0: Added extreme price highlighting for RSI dots

## Support

For questions or issues, please refer to the trading rules documentation or create an issue in this repository.

## License

This project is open source and available under the MIT License. 