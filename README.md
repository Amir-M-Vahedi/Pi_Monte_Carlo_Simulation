# Monte Carlo Simulation to Calculate π

This repository contains a Matlab Live Script implementation of a Monte Carlo simulation to calculate the value of π (pi) with a precision of two decimal places.

<p align="center">
  <img width="700" src="https://github.com/Amir-M-Vahedi/Pi_Monte_Carlo_Simulation/assets/115154998/22ae5891-c195-4c9a-9cfc-fcd35f4f89f3">
</p>

## Project Overview

The Monte Carlo simulation is a statistical method that allows for the estimation of mathematical functions and the modeling of complex systems. In this project, we use the Monte Carlo method to estimate the value of π by simulating random points within a square and counting how many fall inside a quarter circle inscribed within that square.

### Problem Description

The goal is to write a program that uses the Monte Carlo simulation to calculate the value of π with a precision of two decimal places.

#### Approach

1. Consider a quarter circle with a radius of 1 unit, inscribed within a square of side 1 unit.
2. Generate a large number of random points uniformly distributed within the square.
3. Count the number of points that fall inside the quarter circle.
4. The ratio of the number of points inside the quarter circle to the total number of points approximates the ratio of the area of the quarter circle to the area of the square.

Using the relationship between the areas, we get:
<p align="center">
$\lim_{{n \to \infty}} \frac{n_c}{n} = \frac{\frac{1}{4} \pi (1)^2}{1^2} \implies \frac{n_c}{n} \approx \frac{\pi}{4}$
</p>

For a large number of points, \( n \):
<p align="center">
$\pi \approx 4 \times \frac{n_c}{n}$
</p>

where:
- \( $n_c$ \) is the number of points inside the quarter circle.
- \( $n$ \) is the total number of points.
<p align="center">
  <img width="700" src="https://github.com/Amir-M-Vahedi/Pi_Monte_Carlo_Simulation/assets/115154998/9c8ba0aa-8037-47a7-ae6e-44e632e35b3a">
</p>
