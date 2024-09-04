# Dynamics in coiled-coil peptide complexes

### A GitHub repository for "Exchange, promiscuity, and orthogonality in de novo designed coiled-coil peptide assemblies"

**Authors**: Kathleen W. Kurgan, Freddie J. O. Martin, William M. Dawson, Tom Brunnock, Andrew J. Orr-Ewing, and Derek N. Woolfson.

*To whom correspondence should be addressed*: <D.N.Woolfson@bristol.ac.uk>

Check out the preprint [here](https://www.biorxiv.org/content/10.1101/2024.09.01.610678v1)

Please cite: Exchange, promiscuity, and orthogonality in de novo designed coiled-coil peptide assemblies
Kathleen Wilson Kurgan, Freddie James Oliver Martin, William Michael Dawson, Thomas Brunnock, Andrew J Orr-Ewing, Dek N Woolfson
bioRxiv 2024.09.01.610678; doi: https://doi.org/10.1101/2024.09.01.610678.

## About

This repository contains the data and code to analyze (`FEx_dimers_analysis_19APR24.ipynb`) and plot (`FEx_dimer_plots_17JUL24.ipynb`) the concentration and temperature-dependent kinetics of exchange of CC-Di as measured by fluorescence timecourse (see Figure 1).

Data were fit to a single exponent using:

$$
f(t) = A(1 - \exp(k_{\text{obs}} \cdot t))
$$

where $t$ is time, $A$ is the pre-exponential factor, and $k_{\text{obs}}$ is the observed rate.

The activation energy of CC-Di was determined from variable temperature data fit to the Arrhenius equation:

$$
k = A \cdot \exp\left(\frac{-E_a}{RT}\right)
$$

where $k$ is the rate constant, $A$ is the pre-exponential factor, $E_{a}$ ($J$ $mol^{-1}$) is the activation energy, $R$ is the molar gas constant ($J$ $mol^{-1}$ $K^{-1}$), and $T$ is the temperature (K).

This uses the [SciPy](https://scipy.org/) Python package to fit the data. [1]

## References
1) Pauli Virtanen, Ralf Gommers, Travis E. Oliphant, Matt Haberland, Tyler Reddy, David Cournapeau, Evgeni Burovski, Pearu Peterson, Warren Weckesser, Jonathan Bright, Stéfan J. van der Walt, Matthew Brett, Joshua Wilson, K. Jarrod Millman, Nikolay Mayorov, Andrew R. J. Nelson, Eric Jones, Robert Kern, Eric Larson, CJ Carey, İlhan Polat, Yu Feng, Eric W. Moore, Jake VanderPlas, Denis Laxalde, Josef Perktold, Robert Cimrman, Ian Henriksen, E.A. Quintero, Charles R Harris, Anne M. Archibald, Antônio H. Ribeiro, Fabian Pedregosa, Paul van Mulbregt, and SciPy 1.0 Contributors. (2020) SciPy 1.0: Fundamental Algorithms for Scientific Computing in Python. Nature Methods, 17(3), 261-272.

