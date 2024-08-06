# Polymarket Data Fetcher

Polymarket Data Fetcher is a Python package that allows you to easily fetch historical odds data from Polymarket for specific market outcomes.

## Installation

You can install the Polymarket Data Fetcher using pip:
## Usage

Here's a basic example of how to use the Polymarket Data Fetcher:

```python
from polymarket_data_fetcher import PolymarketDataFetcher

# Initialize the fetcher
pm = PolymarketDataFetcher()

# Define the parameters
slug = "will-donald-trump-win-the-2024-us-presidential-election"
start_date = "2024-01-01"  # yyyy-mm-dd format
fidelity = "1440"  # daily data

# Fetch historical odds for a market
odds = pm.get_historical_odds(slug, start_date, fidelity)

# Display the results
print(odds)