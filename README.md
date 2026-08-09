# TradeTrace

## TT Replay v3

`tt-replay-v2` branch contains the current TT Replay implementation for manual FX backtesting.

### Core workflow
- Load 1-hour OHLC CSV exported from MT4 / MT5 / TradingView
- Replay forward without showing future candles
- View D1, H4 and H1 simultaneously
- Use D1 for higher-timeframe context, H4 as the main wave, H1 for entry timing
- Step forward by 1H or 4H, or use autoplay
- Jump to a chosen date/time and reset to that replay starting point
- Add Entry / SL / TP guide lines synced across all three charts
- Save review points with D1 / H4 / H1 notes, decision, result and lesson
- Resume the last replay position with browser local storage
- Export saved review points as JSON
- Responsive layout for iPhone and desktop

### CSV format
A 1-hour CSV is recommended. The parser accepts common Date/Time/Open/High/Low/Close headers and comma, semicolon or tab-separated files.

### Safety
The production `main` branch is not modified by this development branch until the PR is explicitly merged.
