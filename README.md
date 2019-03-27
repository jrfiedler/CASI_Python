# CASI_Python

Python code for _[Computer Age Statistical Inference](https://web.stanford.edu/~hastie/CASI/index.html)_ by Bradley Efron and Trevor Hastie.


## Required packages

- `numpy`
- `pandas`
- `statsmodels`
- `matplotlib`
- `scipy`
- `mpmath` (for section 3.1)

This code was developed with Python 3.7.


## Data

The data can be obtained from the [book site](https://web.stanford.edu/~hastie/CASI/data.html). The notebooks assume that the data has been saved in a `data/` subdirectory.


## Possible errata or differences with the book

- Section 2.1: I get slightly different values for Table 2.1
- Section 6.2, Table 6.3: I get different values for $\hat{sd}$. I get the same values when I drop $x$ from the exponent in Eq 6.21. See [ch06s02.ipynb](chapter06/ch06s02.ipynb).


## To do

- Section 4.3: Figure 4.2
- Section 5.2: Figures 5.2 and 5.3 ?
- Section 6.3


## Contributing

Corrections and contributions are welcome. Please check the list below before submitting contributions.

### DO NOT contribute

- Section 4.1: the calculation of equation 4.10. This is homework exercise 4.1a. This also rules out contributing Figure 4.1
- Section 4.4: Figure 4.3. This would make homework exercise 4.5 trivial.
