# GaussVol

A recursive implementation of Gaussian Molecular Volume algorithm

## References:

Baofeng Zhang, Denise Kilburg, Peter Eastman, Vijay S. Pande, Emilio Gallicchio. Efficient Gaussian Density Formulation of Volume and Surface Areas of Macromolecules on Graphical Processing Units. J. Comp. Chem., 38, 740-752 (2017). [doi:10.1002/jcc.24745] (http://doi.org/10.1002/jcc.24745)

Gallicchio E., and R.M. Levy. AGBNP, an analytic implicit solvent model suitable for molecular dynamics simulations and high-resolution modeling, J. Comp. Chem. 25, 479-499 (2004). [doi:10.1002/jcc.10400](http://doi.org/10.1002/jcc.10400)

Grant, J. A. and Pickup, B. T. A Gaussian Description of Molecular Shape. J. Phys. Chem. 99, 3503 (1995).

## Requires:

OpenMM installation version 7 (for the Vec3 class essentially).

## Compilation and Installation

Assume OpenMM is installed under `/usr/local/openmm`. FIXME: add cmake support
 
```
g++ -shared -fPIC -I/usr/local/openmm/include gaussvol.cpp -o libgaussvol.so
sudo cp libgaussvol.so /usr/local/openmm/lib/
sudo cp gaussvol.h /usr/local/openmm/include/
```
