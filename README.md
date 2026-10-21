# NumMethods · Numerical Analysis Notebooks

**From solving an equation to integrating a temperature model: a collection of numerical methods implemented in Python.**

These notebooks explore how mathematical algorithms behave in code, with symbolic calculations, numerical examples and plots. The collection spans foundational exercises and an applied weather-modeling project.

## Notebook guide

| Notebook | Focus |
|---|---|
| [NumHw1.ipynb](NumHw1.ipynb) | Root-finding exercises, including bisection, Newton and secant methods |
| [NumHW2.ipynb](NumHW2.ipynb) | Lagrange/Neville/divided-difference interpolation, finite differences, Richardson extrapolation, quadrature and ODE solvers |
| [ProjectNumMeth1.ipynb](ProjectNumMeth1.ipynb) | Temperature modeling using weather data, solar geometry and a Runge–Kutta implementation |

The second notebook includes Euler, Taylor and fourth-order Runge–Kutta methods, making it useful for comparing how different update rules approximate a differential equation.

## Open locally

Create and activate a Python environment, then install Jupyter and the core scientific libraries:

```bash
python -m pip install jupyterlab numpy pandas matplotlib sympy
python -m jupyter lab
```

The weather project additionally imports Meteostat and Astral. Review its installation cells and data-access assumptions before running it. Some cells ask for input or reuse variables created earlier, so follow the notebook order.

## A useful way to read the exercises

For each method, identify the input assumptions, stopping rule and source of numerical error. Try changing the initial bracket, starting point or step size and compare the result with a known reference where available.

The notebooks are coursework and exploratory implementations, rather than a general-purpose numerical library. There is no pinned environment or uniform convergence guarantee across the examples.

## From notebook to interface

The weather-modeling direction continues in [Atmos / WeatherPrediction](https://github.com/FyodorAmanov1/WeatherPrediction), which provides an interactive browser dashboard, a revised RK4 temperature model and explicit comparison with a persistence baseline.
