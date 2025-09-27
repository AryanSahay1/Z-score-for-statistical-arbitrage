# Z-score-for-statistical-arbitrage
“A beginner-friendly statistical arbitrage (pairs trading) model using Z-Score. It identifies when two assets move too far apart, generates buy/sell signals, and backtests performance with clear visualizations.”

📊 Z-Score Statistical Arbitrage (Pairs Trading Strategy)

This project is a simple but powerful way of finding trading opportunities by looking at how two assets (like two stocks or currencies) usually move together. If they get “too far apart” from their normal relationship, this model helps spot those moments and suggests when to buy one and sell the other.

🌍 What is Statistical Arbitrage?

Think of two best friends who usually walk side by side at the same pace. Most of the time, they stay close. But sometimes, one walks ahead too fast, while the other lags behind. Sooner or later, the one ahead slows down, and the other catches up — they come back together.

Now replace those friends with two assets (like stocks or forex pairs). They usually move together, but when they separate too much, that gap is a trading opportunity.

If one asset goes too high compared to the other → sell the high one

If the other asset goes too low → buy the low one

When they come back together, you make a profit.

That’s statistical arbitrage, and more specifically, pairs trading. It’s called market-neutral, because it doesn’t matter if the overall market is going up or down — you only care about the relationship between the two assets.

📌 What This Project Does

This notebook is built around the Z-Score method, which is a way of measuring how far something is from its average.

Here’s what the model does in simple steps:

Collect data → Pulls historical price data from Yahoo Finance for two assets.

Calculate the spread → Finds the difference between the two prices (this is like measuring the gap between our “two friends”).

Use Z-Score → Converts the spread into standard deviations. This helps us see when the spread is “too high” or “too low” compared to normal.

Create trading signals →

If the spread is way above normal → the model suggests selling the expensive asset.

If the spread is way below normal → the model suggests buying the cheap asset.

Backtest → Tests the idea on past data to see if it would have made money.

Show results → Plots graphs so you can clearly see spreads, Z-Scores, and where trades happened.

🎯 Why This is Useful

Easy to understand → A beginner-friendly way to learn about algorithmic trading.

Practical strategy → This same idea is used in hedge funds and quant firms worldwide.

Market-neutral → Works in rising or falling markets because it focuses on relative movement.

Great for learning → If you’re new to finance or data science, this project is a hands-on way to understand how real trading strategies are built.

🛠 Tools & Libraries

Python (Google Colab) – main language and environment

yfinance – fetches real market data

Pandas & NumPy – for calculations and data handling

Matplotlib – for plotting graphs and signals

🚀 Future Plans

Expand the strategy to multiple pairs at once

Add smarter models like Kalman Filters or Hidden Markov Models

Connect it with broker APIs for live trading

👤 Author: Aryan Sahay
⚠️ Disclaimer: This project is for research and educational purposes only. It is not financial advice.
