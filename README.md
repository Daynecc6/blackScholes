# Black-Scholes Option Pricing Model

This repository contains a Python implementation of the Black-Scholes option pricing model. The Black-Scholes model is a mathematical model used to calculate the theoretical price of European-style options.

## Features

- Calculate prices for both call and put options
- Easy-to-use function with clear parameters
- Utilizes SciPy for statistical calculations

## Requirements

- Python 3.x
- SciPy

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/black-scholes-model.git
   ```
2. Install the required package:
   ```
   pip install scipy
   ```

## Usage

Here's a basic example of how to use the `black_scholes` function:

```python
from black_scholes import black_scholes

S = 100    # Current stock price
K = 100    # Strike price
T = 1      # Time to maturity in years
r = 0.05   # Risk-free interest rate
sigma = 0.2  # Volatility

call_price = black_scholes(S, K, T, r, sigma, option_type='call')
put_price = black_scholes(S, K, T, r, sigma, option_type='put')

print(f"Call Option Price: {call_price:.2f}")
print(f"Put Option Price: {put_price:.2f}")
```

## Function Parameters

- `S`: Current stock price
- `K`: Option strike price
- `T`: Time to maturity (in years)
- `r`: Risk-free interest rate (annual)
- `sigma`: Volatility of the underlying stock (annual)
- `option_type`: 'call' for call option, 'put' for put option
