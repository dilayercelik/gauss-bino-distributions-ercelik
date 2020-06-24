# gauss-bino-distributions-ercelik

# About
This is a Python package with which you can calculate Binomial and Gaussian distributions with given data, and the probability distribution functions associated with Gaussian and Binomial distributions (PDF). 

It can be used to plot graphs (histogram, bar chart) associated with the probability disributions and the probability density distributions.

See the Usage section for an example usage.

# Files
setup.py - file necessary for pip installing

gauss_bino_distributions - folder with the files that make up the Python package

# Prerequisites 
This package requires:
- python3 

- matplotlib package

- math package


# Installation
## Install with pip:

```bash
pip install gauss-bino-distributions-ercelik`
```

## To upgrade the package:

```bash
pip install gauss-bino-distributions-ercelik --upgrade`
```

# Usage

```python
import gauss_bino_distributions_ercelik as gbd

# instances of Gaussian and Binomial classes
gaussian_example = gbd.Gaussian()  # creates a Gaussian object with default mu = 0 and sigma = 1

binomial_example = gbd.Binomial()  # creates a Binomial object with default p = 0.5 and n = 25

# plots a histogram of the instance variable data (Gaussian)
gaussian_example.plot_histogram()

# plots a bar chart of the data set (Binomial)
binomial_example.plot_bar()

# Probability density function calculator for the gaussian distribution
gaussian_example.pdf(0.7)

# Probability density function calculator for the binomial distribution
binomial_example.pdf(3)

# plots of the probability density function (gaussian)
gaussian_example.plot_histogram_pdf(n_spaces = 50)

# plots the probability density function (binomial)
binomial_example.plot_pdf()

# adds together two Gaussian distributions
gaussian_2 = Gaussian(2, 7)  # example of second Gaussian object

gaussian_example + gaussian_2  # returns another Gaussian object with its own mean and standard deviation

# adds together two Binomial distributions with equal p
binomial_2 = Binomial(0.5, 29) # example of second Binomial object - same p as binomial_example object

binomial_example + binomial_2. # returns another Binomial object 
```


# Author
Dilay Fidan Ercelik

# Acknowledgment
This package was put together thanks to the lessons provided at Udacity - Machine Learning Foundations Free Course.

# License
MIT License - see [LICENSE.txt](https://github.com/dilayercelik/gauss-bino-distributions-ercelik/blob/master/LICENSE.txt)
