# CS 7389H — Advanced Deep Learning
### Texas State University · Fall 2026

Course materials: lecture notebooks, assignments, and supporting code.

**Textbook:** Simon J. D. Prince, *Understanding Deep Learning*, MIT Press, 2023 —
freely available at [udlbook.com](https://udlbook.com).

## Layout

    notebooks/                 background and lecture notebooks
    assignments/               assignments, one folder each
    data/                      small datasets and images the notebooks read
    output/                    scratch space for files your code writes (10.5 downloads MNIST here)

## Background notebooks

Chapter 1 of the textbook assumes a working knowledge of undergraduate mathematics.
These four notebooks review it. Work through them before attempting Assignment 1.

| notebook | topics |
|---|---|
| `notebooks/01.1-math_for_ml-basic_algebra.ipynb` | equations, functions, graphing |
| `notebooks/01.2-math_for_ml-linear_algebra.ipynb` | vectors, matrices, rank, transformations |
| `notebooks/01.3-math_for_ml-calculus.ipynb` | limits, derivatives, critical points, partial derivatives, integration |
| `notebooks/01.4-math_for_ml-stats_and_proba.ipynb` | descriptive statistics, distributions, probability, hypothesis testing |

## Lecture notebooks

One or more notebooks accompany each chapter of the textbook, numbered by chapter (notebook 6.3 goes with Chapter 6). Most are adapted from the book's official notebooks at [github.com/udlbook/udlbook](https://github.com/udlbook/udlbook). Cells marked "TO DO" ask you to write code or to predict what will happen before you run the next cell.

| chapter | notebooks | topics |
|---|---|---|
| 2. Supervised learning | 2.1, 2.2 | linear regression, loss, fitting; worked examples on real data |
| 3. Shallow neural networks | 3.1 to 3.4 | 1D and 2D inputs, linear regions, activation functions |
| 4. Deep neural networks | 4.1 to 4.3 | composing networks, clipping functions, matrix form |
| 5. Loss functions | 5.1 to 5.3 | least squares, binary and multiclass cross-entropy |
| 6. Fitting models | 6.1 to 6.5 | line search, gradient descent, SGD, momentum, Adam |
| 7. Gradients and initialization | 7.1 to 7.3 | backpropagation in a toy model and a deep network, initialization |
| 8. Measuring performance | 8.1 to 8.4 | MNIST-1D, bias-variance trade-off, double descent, high-dimensional spaces |
| 9. Regularization | 9.1 to 9.5 | L2 regularization, implicit regularization, ensembling, Bayesian approach, augmentation |
| 10. Convolutional networks | 10.1 to 10.5 | 1D and 2D convolution, a CNN for MNIST-1D, downsampling and upsampling, a CNN for MNIST |

A few notebooks need more than the packages listed under Requirements:

- 8.1, 8.3, 9.5, and 10.2 use the MNIST-1D dataset. Their first code cell installs the `mnist1d` package, and the dataset is generated and saved the first time you run them.
- 10.4 reads `data/test_image.png` (on Colab it downloads the image instead).
- 10.5 downloads MNIST (about 11 MB, 64 MB once unpacked) into `output/` the first time you run it, so be online for that cell.
- 8.3 and 10.5 train on a GPU when PyTorch can find one and on the CPU otherwise. On Google Colab, choose *Runtime → Change runtime type → T4 GPU* first.

## Assignments

| assignment | notebook | points |
|---|---|---|
| 1 — Basic Mathematics for Deep Learning | `assignments/assignment1/assignment1.ipynb` | 100 |

Download the notebook, fill it in, run it top to bottom (*Kernel → Restart & Run All*), and
upload the completed `.ipynb` to Canvas. Submission instructions are in the notebook itself.

## Requirements

    python >= 3.10, numpy, matplotlib, pandas, scipy, statsmodels, torch, torchvision, pillow, mnist1d

Assignment 1 downloads a dataset over the network the first time you run its Q4.2, so be
online for that cell.
