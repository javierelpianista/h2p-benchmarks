# Contents of this SI

For the quantum numbers that label each state, we follow all the definitions of http://dx.doi.org/10.1016/s0065-2199(08)60183-9.
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

## Accurate benchmark values for selected cases

These values are located in file `benchs.dat`.
Each line contains the values of `l`, `m`, `I`, followed by `E` and `A`.

## Equilibrium internuclear distance, electronic + nuclear energy, and separation constant

These values are located in file `req.dat`.
Each line contains the values of `l`, `m`, `I`, followed by `U`, `A`, and `R`, where `U` is the electronic + nuclear energy `U = E + 1/R`.
