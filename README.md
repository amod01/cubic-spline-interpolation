# Cubic Spline Interpolation for Yield Curve

This repository contains two Python scripts that perform cubic spline interpolation on yield curve data. Both scripts achieve the same goal of interpolating yield rates for given time-to-maturity data but use different methods to accomplish this.

---

## Files

1. **Manual Cubic Spline Interpolation (`manual_cubic_spline.py`)**
   - Implements a manual cubic spline interpolation algorithm from scratch.
   - Calculates coefficients for cubic spline segments and evaluates the spline at specified points.
   - Plots the interpolated yield curve and finds the yield rate at a specific maturity (e.g., 4 years).

2. **Scipy Cubic Spline Interpolation (`scipy_cubic_spline.py`)**
   - Uses the `CubicSpline` class from the `scipy.interpolate` module for interpolation.
   - Simplifies the interpolation process using built-in `scipy` functionality.
   - Plots the interpolated yield curve and finds the yield rate at a specific maturity (e.g., 4 years).

---

## How These Methods Achieve the Same Goal

Both scripts interpolate yield rates for given time-to-maturity data using cubic spline interpolation. Here's how they differ:

### Manual Cubic Spline Interpolation
- **Algorithm Implementation**: Manually implements the cubic spline interpolation algorithm, including coefficient calculations.
- **Custom Functions**: Defines functions to set up and solve the tridiagonal system, compute coefficients, and evaluate the spline.
- **Flexibility**: Provides a deeper understanding of the underlying mathematics and allows for customization.

### Scipy Cubic Spline Interpolation
- **Library Usage**: Uses the `CubicSpline` class from `scipy.interpolate`, abstracting away complexity.
- **Ease of Use**: Concise and easy to implement, leveraging optimized `scipy` functions.
- **Efficiency**: Highly optimized for performance, suitable for large datasets.
