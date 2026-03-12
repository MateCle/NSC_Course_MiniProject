# NSC Mini-Project: The Mandelbrot Set

**Course:** Numerical Scientific Computing (Spring 2026)  
**University:** Aalborg University Copenhagen (AAU CPH)
**Student Name:** Matteo Clementin

## Project Overview
This repository contains the first mini-project for the Numerical Scientific Computing course. The goal of this project is to compute the Mandelbrot set fractal and conduct a rigorous performance scaling analysis across three different Python implementations:
1. **Naive:** Pure Python nested loops.
2. **NumPy:** Vectorized implementation using broadcasting and boolean masking.
3. **Numba:** Just-In-Time (JIT) compiled implementation.

The project demonstrates key computer architecture concepts such as algorithmic intensity, memory-bound vs. compute-bound kernels, cache spatial/temporal locality, and the elimination of interpreter overhead.

## Repository Structure
- `Mandelbrot_set.ipynb`: The main Jupyter Notebook serving as both the source code and the academic report. It contains the implementations, visualizations, benchmarking loop, and the final hardware-level reasoning.
- `timing_results.csv`: The exported dataset containing the raw execution times and computed speedups for varying grid resolutions (from 100x100 to 1500x1500).
- `git_log.txt`: The development history log formatted as required by the assignment guidelines.

## Dependencies
To run the notebook, ensure you have Python 3 installed along with the following libraries:
```bash
pip install numpy numba matplotlib pandas jupyter