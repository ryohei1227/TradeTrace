# TradeTrace 2.0

TradeTrace 2.0 is a mobile-first trading research journal with two clearly separated workflows.

## Backtest Research

Stores annual backtest results by year, market, and symbol/pair, including:

- Initial balance
- Net profit
- Gross profit / gross loss
- Profit factor
- Expectancy
- Win rate
- Maximum drawdown (amount / %)
- Absolute drawdown
- Number of trades
- Average winning / losing trade
- Research notes
- Daily, 4H, 1H chart images and an optional result screenshot

Large chart images are resized and JPEG-compressed in the browser before being stored locally in IndexedDB.

## Live Trading Journal

A separate journal for real-trade review, including:

- Date, market, pair/symbol, direction and result
- P/L, entry/exit, stop, planned/actual RR
- Rule adherence
- Emotion before/after the trade
- Daily / 4H / 1H reasoning
- Entry or skip rationale
- Lesson / next adjustment
- Daily, 4H, 1H and optional result screenshots

The local review intentionally prioritizes process quality and rule adherence over whether a single trade won or lost.

## Data and privacy

Trade records and compressed images are stored in the browser using IndexedDB. The static GitHub Pages build does not automatically upload chart images to a server. JSON export/import is available for backups.

## AI image analysis limitation

The current GitHub Pages-only build can save and preview chart screenshots and can evaluate numerical/statistical inputs locally. It does not send chart images to a multimodal AI model. True chart-image AI analysis will require a future API/backend integration or sharing the saved images with ChatGPT.

## Branch

TradeTrace 2.0 development is isolated on `tradetrace-v2`. The `main` branch is not modified until the pull request is reviewed and merged.
