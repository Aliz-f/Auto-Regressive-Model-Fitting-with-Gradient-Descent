# Auto-Regressive Model Fitting with Gradient Descent

This project fits auto-regressive (AR) models using both regular and stochastic gradient descent techniques. The analysis uses two given time series datasets, with a focus on estimating model parameters, comparing gradient descent methods, and exploring the impact of different learning rates on training error convergence.

## Experiment Overview
The AR(2) model used in this study is defined as:
$x(n) = -w_1 x(n - 1) - w_2 x(n - 2) + \epsilon(n)$
where:
- $x(n)$ is the time series data.
- $x(n - 1)$ and $x(n - 2)$ are the lag 1 and lag 2 series.
- $\epsilon(n)$ represents Gaussian noise with zero mean.

### Steps Involved
1. **Data Preparation:**
   - Construct lag series $x(n - 1)$ and $x(n - 2)$ by filling the lag vectors with zeros to maintain a length of 1000 for consistency.

2. **Model Fitting:**
   - **(a)** Estimate parameters $w_1$ and $w_2$ for the two datasets using regular gradient descent.
   - **(b)** Apply stochastic gradient descent and compare results with part (a).

3. **Training Error Analysis:**
   - **(c)** Plot training error as a function of the iteration step using 3 different learning rates with regular gradient descent on dataset 1.
   - **(d)** Plot training error with stochastic gradient descent using 3 different learning rates on dataset 1.
   - **(e)** Compare the convergence patterns between regular and stochastic gradient descent.

## Results
- Final values for $w_1$ and $w_2$ for both regular and stochastic gradient descent methods on both datasets.
- Visual comparison of training errors across different learning rates.

## Dependencies
- Python 3.x
- Jupyter Notebook
- Required libraries: `numpy`, `matplotlib`, `pandas`

## How to Run
1. Clone the repository: `git cloen https://github.com/Aliz-f/Auto-Regressive-Model-Fitting-with-Gradient-Descent`
2. Install the required libraries: `pip install numpy matplotlib pandas`
3. Open the Jupyter Notebook

## License
This project is licensed under the MIT License.
