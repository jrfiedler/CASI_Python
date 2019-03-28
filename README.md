# CASI_Python

Python code for _[Computer Age Statistical Inference](https://web.stanford.edu/~hastie/CASI/index.html)_ by Bradley Efron and Trevor Hastie.


## Required packages

- `numpy`
- `pandas`
- `statsmodels`
- `matplotlib`
- `scipy`
- `mpmath` (for section 3.1)
- `sklearn` (scikit-learn)
- `graphviz` (for section 8.4)

This code was developed with Python 3.7.


## Data

The data can be obtained from the [book site](https://web.stanford.edu/~hastie/CASI/data.html). The notebooks assume that the data has been saved in a `data/` subdirectory.


## Possible errata or differences with the book

- Section 2.1: I get slightly different values for Table 2.1
- Section 6.2, Table 6.3: I get different values for $\hat{sd}$. I get the same values when I drop $x$ from the exponent in Eq 6.21. See [ch06s02.ipynb](chapter06/ch06s02.ipynb).
- Section 7.1, eq 7.12: Is $\hat{B}$ missing a $\sigma^2$?
- Section 7.2: I think eq 7.23 should actually be $\displaystyle \hat{p}^{\text JS}_i = \frac{1}{n}\left[(n + 0.75) \sin^2 \left(\frac{\hat{\mu}^{\text JS}_i}{2 \sqrt{n + 0.5}}\right) - 0.375 \right] $
- Section 7.4: Eq 7.46 is missing "1/1000", i.e., it isn't taking the mean
- Section 8.3:
    - The data page says the values in the galaxy dataset are log-redshift, but they are likely log-log-redshift, if 1.22 \leq r \leq 3.32 as equation 8.38 says
    - Equation 8.38 says 17.2 \leq m \leq 21.5, but the y-axis on figure 8.5 shows negative values, approximately -21 \leq m \leq -17
- Section 10.4, pg 171: Equation 10.55 might give the impression that the powers of the bin counts are used in the model (i.e., that the $\hat{\beta}$ values are coefficients from the model). In fact, orthogonal polynomials are used. See [ch10s04.ipynb](chapter10/ch10s04.ipynb).


## To do

- Section 4.3: Figure 4.2
- Section 5.2: Figures 5.2 and 5.3 ?
- Section 6.3
- Section 8.4: Figure 8.7 doesn't completely match the book
- Section 10.5: Infinitesimal jackknife / influence function s.e. for Table 10.2


## Contributing

Corrections and contributions are welcome. Please check the list below before submitting contributions.

### DO NOT contribute

- Section 4.1: the calculation of equation 4.10. This is homework exercise 4.1a. This also rules out contributing Figure 4.1
- Section 4.4: Figure 4.3. This would make homework exercise 4.5 trivial.
- Section 7.2: entire section. Calculating the JS estimates is exercise 7.3
- Section 7.3: sd values in Table 7.3. This is exercise 7.7a
- Section 7.4: entire section, probably. The section mainly uses JS estimates, and calculating those estimates is exercise 7.3
- Section 8.1: Figure 8.2, Table 8.1, and Table 8.2. These are covered by exercises 8.1 and 8.3.
- Section 8.3: entire section, probably; covered by exercise 8.6
- Section 9.2: Figure 9.2; would probably make exercise 9.3 trivial
- Section 9.3: Table 9.4? Might make exercise 9.4 too easy.
- Section 9.5: Table 9.8; covered by exercise 9.7
- Section 10.2: Figure 10.2; covered by exercise 10.3
