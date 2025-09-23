# Inaccurate Options Pricing Calculator with Greeks
This project was originally implemented with LibreOffice's Calc (calc is short for calculator, hence the repository name) as a tool to determine European-style call and put option prices and greeks using the Black-Scholes-Merton model.
I found this tool quite useful to some European-style non-collateralized cash-settled structured call and put warrants which are listed on Bursa Malaysia Securities Berhad ("Bursa Securities").

## Notes
The Risk-Free Interest Rate, Dividend Yield, and Volatility are annualized. The calculation for the Theoretical Values is based on the [Black-76 model.](https://en.wikipedia.org/wiki/Black_model) The approximation for the of the standard normal cumulative distribution function (CDF) N(x) in the calculation used is specifically the [Abramowitz and Stegun approximation](https://personal.math.ubc.ca/~cbm/aands/frameindex.htm) with approximately 10⁻⁷ max absolute error, which is far from the more optimized modern state-of-the-art approximation methods, hence "Inaccurate." 

In addition, the Black-Scholes-Merton model is not the most accurate or widely used model in practice for complex or real-world option pricing. In professional settings, more advanced modern benchmarks such as the stochastic volatility models, jump-diffusion models, local volatility models, and volatility surface modeling, have largely replaced it for accurate pricing and risk management. Not financial advice btw.

## Resources
1. Moa, Fabian. (2020, April 18). *Building a Black-Scholes-Merton (BSM) Option Pricing Calculator (with Greeks)*. Retrieved from https://fabianmoa.com/2020/04/18/building-a-black-scholes-merton-bsm-option-pricing-calculator-with-greeks\

