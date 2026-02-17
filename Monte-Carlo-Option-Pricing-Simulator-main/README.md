# Monte Carlo Option Pricing Simulator

[![Python Version](https://img.shields.io/badge/python-3.7%2B-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> A professional simulator for pricing European options using Monte Carlo methods, with a visual comparison to the Black-Scholes analytical model.

This project simulates stock price paths using Geometric Brownian Motion (GBM) to price European Call and Put options. It serves as an educational tool for finance, research, and quantitative analysis, providing animated visualizations of the simulations.

## Table of Contents

- [Features](#features)
- [Formulas](#formulas)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

-   **Stock Price Simulation**: Simulates future stock price paths using Geometric Brownian Motion.
-   **Monte Carlo Pricing**: Prices European Call and Put options based on the simulated paths.
-   **Black-Scholes Comparison**: Calculates the analytical Black-Scholes price for comparison.
-   **Animated Visualization**: Animates the stock price paths and the convergence of the Monte Carlo price.
-   **Professional UI**: A clean, dark-themed interface for a better user experience.

## Formulas

### Geometric Brownian Motion (GBM)

The evolution of the stock price is modeled as:
$$
S_t = S_0 \exp\left((r - 0.5\sigma^2)t + \sigma W_t\right)
$$
Where:
-   $S_t$: Stock price at time $t$
-   $S_0$: Initial stock price
-   $r$: Risk-free rate
-   $\sigma$: Volatility
-   $W_t$: Wiener process (Brownian motion)

### Black-Scholes Formula

The analytical price of a European option is given by:

**Call Price:**
$$
C = S_0 N(d_1) - K e^{-rt} N(d_2)
$$

**Put Price:**
$$
P = K e^{-rt} N(-d_2) - S_0 N(-d_1)
$$

Where:
$$
d_1 = \frac{\ln(S_0/K) + (r + 0.5\sigma^2)t}{\sigma\sqrt{t}}
$$
$$
d_2 = d_1 - \sigma\sqrt{t}
$$

## Tech Stack

-   Python
-   NumPy
-   SciPy
-   Matplotlib

## Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/AbhiramSharma/Monte-Carlo-Option-Pricing-Simulator.git
    cd Monte-Carlo-Option-Pricing-Simulator
    ```

2.  **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

To run the simulation, execute the following command:

```bash
python main.py
```

The simulation parameters (strike price, volatility, etc.) are clearly labeled and visualized in the plot.

## File Structure

-   `main.py`: The main entry point for handling the simulation, visualization, and price comparison.
-   `utils.py`: Contains the core functions for GBM simulation and option pricing.
-   `requirements.txt`: A list of the Python dependencies for the project.
-   `README.md`: This file.

## Contributing

Contributions are welcome! If you have ideas for new features or improvements, feel free to fork the repository and submit a pull request.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.

## Contact

Abhiram Sharma - ab23.ar39@gmail.com

Project Link: [https://github.com/AbhiramSharma/Monte-Carlo-Option-Pricing-Simulator](https://github.com/AbhiramSharma/Monte-Carlo-Option-Pricing-Simulator)
