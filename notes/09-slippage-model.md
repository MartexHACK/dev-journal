# Model slippage before believing any backtest

A strategy with a 4 basis point per-trade edge and 200 trades a year dies at 5 basis points of slippage. Slippage should scale with order size relative to displayed depth, not sit as a flat constant. Backtests that use a flat cost systematically favour high-turnover strategies.
