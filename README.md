# stochastic-flood-simulation

Monte Carlo simulation of flood events using non-homogeneous Poisson processes.

---

## Overview

This project studies flood risk using stochastic simulations and probabilistic modeling.

The objective is to estimate the probability of a flood event caused by random rainfall intensities over time.

The model combines:

- non-homogeneous Poisson processes,
- rainfall intensity simulation,
- rejection sampling methods,
- Monte Carlo estimation,
- variance reduction techniques,
- performance optimization using vectorization and C++.

The project was developed as part of a simulation techniques course.

---

## Mathematical Model

Rainfall events are modeled using a non-homogeneous Poisson process with intensity:


$$\lambda(t) = \lambda_0 (1 + \alpha \sin(4\pi t))$$

Rain intensities are simulated from a custom probability density using rejection sampling.

The river height evolution is modeled by:


$$ H(t) = \sum_i I_i e^{-v(t-T_i)}$$

where:

- $T_i$ are rainfall dates,
- $I_i$ are rainfall intensities,
- $v$ controls water absorption.

A flood occurs when:


$$ H(t) > h_0$$


---

## Main Features

- Simulation of rainfall intensities
- Non-homogeneous Poisson process simulation
- Flood probability estimation
- Importance sampling for rare events
- Vectorized Monte Carlo simulations
- Contral Variate for the variance reduction

---

## Technologies
 Python / Jupyter Notebook
