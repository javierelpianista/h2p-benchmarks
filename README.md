[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5044229.svg)](https://doi.org/10.5281/zenodo.5044229)

# Contents 

This repository contains benchmark electronic energy `E`, separation constant `A` and internuclear separation `R` values of the hydrogen molecule cation computing using the Riccati-Padé method (RPM) [[1]](https://doi.org/10.1002%2Fslct.202102509).
It also contains values for the electronic plus nuclear repulsion energy `U = E + 1/R`, and its derivative with respect to `R` for a few selected states.

For the quantum numbers that label each state, we follow all the definitions of [[2]](https://dx.doi.org/10.1016/s0065-2199(08)60183-9).
Briefly, the quantum numbers used here are:

* `l`: (quantum) number for the angular momentum in the united-atom limit
* `m`: quantum number for the z-component of the angular momentum
* `I`: number that distinguishes states with the same m and l

Some relations they follow:

* `I = nu - l = Nl + 1`, where `nu` is the total quantum number in the united-atom limit, and `Nl` is the number of nodes `L(lambda)` has. 
* `Nm = l - |m|`, where `Nm` is the number of nodes that `M(mu)` has
* `t` is set to 0 when `Nm` is even, and to 1 when `Nm` is odd

## Dissociation curves

The dissociation curves are provided for 69 states in the folder `discurves/`.
Each state is named `l_m_I.dat`, and each line contains `R`, `E`, and `A`.
Even though `R` is reported to only 2 significant digits, this is only done for better formatting, but they are exact.
The values of `E` and `A` are reported with the correct number of significant digits, measured by comparing the results of the computation with the last two values of `D`.

## Electronic + nuclear repulsion energy derivatives

The dissociation curves `U` and its derivative with respect to `R` are provided in the folder `discurves_with_derivative/`.
Each state is named in the same way as in the previous section, and each line contains `R`, `U`, `dU/dR`, and `A`.

## Accurate benchmark values for selected cases

These values are located in file `benchs.dat`.
Each line contains the values of `l`, `m`, `I`, followed by `E` and `A`.

## Equilibrium internuclear distance, electronic + nuclear energy, and separation constant

These values are located in file `req.dat`.
Each line contains the values of `l`, `m`, `I`, followed by `U`, `A`, and `R`, where `U` is the electronic + nuclear energy `U = E + 1/R`.
Benchmark values of the electronic energy, separation constant and internuclear distances for the hydrogen molecule cation

## References
[1] Fernández, F. M., Garcia, J., *ChemistrySelect* **2021**, *6*, 9527-9534.

[2] Bates, D. R., Reid, R. H. G., in *Advances in Atomic and Molecular Physics*, Elsevier, **1968**, 13-35.

Shield: [![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
