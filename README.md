# CS 7389H — Advanced Deep Learning
### Texas State University · Fall 2026

Course materials: lecture notebooks, assignments, and supporting code.

**Textbook:** Simon J. D. Prince, *Understanding Deep Learning*, MIT Press, 2023 —
freely available at [udlbook.com](https://udlbook.com).

## Layout

    notebooks/                 background and lecture notebooks
    assignments/               assignments, one folder each
    output/                    scratch space for files your code writes

## Background notebooks

Chapter 1 of the textbook assumes a working knowledge of undergraduate mathematics.
These four notebooks review it. Work through them before attempting Assignment 1.

| notebook | topics |
|---|---|
| `notebooks/01.1-math_for_ml-basic_algebra.ipynb` | equations, functions, graphing |
| `notebooks/01.2-math_for_ml-linear_algebra.ipynb` | vectors, matrices, rank, transformations |
| `notebooks/01.3-math_for_ml-calculus.ipynb` | limits, derivatives, critical points, partial derivatives, integration |
| `notebooks/01.4-math_for_ml-stats_and_proba.ipynb` | descriptive statistics, distributions, probability, hypothesis testing |

## Assignments

| assignment | notebook | points |
|---|---|---|
| 1 — Basic Mathematics for Deep Learning | `assignments/assignment1/assignment1.ipynb` | 100 |

Download the notebook, fill it in, run it top to bottom (*Kernel → Restart & Run All*), and
upload the completed `.ipynb` to Canvas. Submission instructions are in the notebook itself.

## Requirements

    python >= 3.10, numpy, matplotlib, pandas, scipy, statsmodels

Assignment 1 downloads a dataset over the network the first time you run its Q4.2, so be
online for that cell.
