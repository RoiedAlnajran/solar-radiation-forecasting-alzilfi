# Solar Radiation Forecasting, Al-Zilfi, Saudi Arabia

A systematic evaluation of 52 published global solar radiation models against
7-year averaged data for Al-Zilfi, Saudi Arabia, followed by locally calibrated
regression modeling. Conducted as a research internship at KACST under the
supervision of Prof. Zaki Almustafa.

**Key result:** The locally calibrated quadratic model achieves an RMSE of
**0.0189**, a 65% improvement over the best-performing global model (RMSE=0.0547).

## What This Project Does

Most solar radiation forecasting models are calibrated for temperate climates and
perform poorly in arid regions like central Saudi Arabia. This project:

1. Applies 52 global models to Al-Zilfi data and evaluates each on 4 error metrics
   (MBE, RMSE, MPE, MABE)
2. Identifies models unsuitable for the region using a ±10% acceptance band
3. Develops a locally calibrated model by testing 7 regression types
   (linear, quadratic, cubic, quartic, logarithmic, exponential, power)
4. Selects the quadratic model as the best balance of accuracy and parsimony

## Selected Model

$$\frac{H}{H_0} = 0.4114\left(\frac{S}{S_0}\right)^2 - 0.4665\left(\frac{S}{S_0}\right) + 0.7319$$

Where H/H₀ is the clearness index and S/S₀ is the relative sunshine duration.

## Results

| Metric | This Study | Best Global Model (JAIN11) |
|--------|-----------|--------------------------|
| RMSE   | **0.0189** | 0.0547 |
| MBE    | **≈ 0.000** | −0.053 |
| R²     | **0.980** | — |
| MPE    | **0.10%** | −1.53% |

## Limitations

With only 12 monthly data points (7-year averages), high R² is expected for any
smooth regression. Results represent a preliminary regional calibration, not a
statistically robust generalizable model. A larger dataset would be required for
validation.

## Skills Demonstrated

`Python` `NumPy` `Pandas` `Matplotlib` `Regression Analysis`
`Scientific Computing` `Data Visualization` `Research Methodology`

## Study Location

Al-Zilfi, Riyadh Region, Saudi Arabia — 26.3°N, 44.8°E, Altitude 605m
