# Objective

Framework to run just the intraday strategies. But keep it open for extension.

## tasks

### in-progress tasks

- start data sources in the morning.
- run scheduled tasks in the morning (to collect nse and bank nifty data only for now)
- engine should remove the scheduled tasks after office hours (to stop fetching data)
- the system should not run on holidays.

### backlog tasks

#### CODE IMPROVEMENT

- create data provider and move the logic out of engine.

#### STRATEGY IMPROVEMENTS

- wrong sl issue in fiveEMA strategy.
- add hovertext to shapes.
- add capability to exit when sl is reached and same for entry.

#### NEW FEATURE

- send order updates to telegram.

#### API

- Add database before doing anything on the api side.
- be able to retrieve the candlestick data from data source using api.
- add support to fetch orders placed by a strategy for a run.

### DONE TASKS

- add logging to file handler.

## system design

there will be strategy runs (backtesting | live), it has to be handled separately.
ability to analyze each run.
strategy will keep on evolving.
