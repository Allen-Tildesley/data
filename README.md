# Data
This data was created in 2017
by Michael P. Allen <m.p.allen@warwick.ac.uk>/<m.p.allen@bristol.ac.uk>
and Dominic J. Tildesley <d.tildesley7@gmail.com> ("the authors"),
to accompany the book
[Computer Simulation of Liquids](https://global.oup.com/academic/product/computer-simulation-of-liquids-9780198803201),
second edition, 2017 ("the text"),
published by Oxford University Press ("the publishers").

## Licence
Creative Commons CC0 Public Domain Dedication.
To the extent possible under law, the authors have dedicated all copyright and related
and neighboring rights to this data to the PUBLIC domain worldwide.
This data is distributed without any warranty.
You should have received a copy of the
[CC0 Public Domain Dedication](./COPYING.txt)
along with this data.
If not, see <http://creativecommons.org/publicdomain/zero/1.0/>.

## Disclaimer
The authors and publishers make no warranties about the data, and disclaim liability
for all uses of the data, to the fullest extent permitted by applicable law.
The authors and publishers do not recommend use of this data for any purpose.
It is made freely available, solely to clarify points made in the text.
When using or citing the data, you should not imply endorsement by the authors or publishers.

## Pair distribution function (pair_distribution)
Here we provide data suitable to test the programs `pair_distribution.f90` and `pair_distribution.py`,
which are available in the [Examples repository](https://github.com/Allen-Tildesley/examples).
The file `pair_distribution_data.zip` contains
a set of 500 configurations
of _N_=256 Lennard-Jones atoms,
cut (but not shifted) at _R_<sub>c</sub>=2.5&sigma;,
at the usual state point &rho;=0.75, _T_=1.0.
The interval between configurations was 100 MC sweeps.
For more details about the programs,
and a plot of the results from this data set,
refer to the [Fortran GUIDE](https://github.com/Allen-Tildesley/examples/blob/master/GUIDE.md)
or the [Python GUIDE](https://github.com/Allen-Tildesley/examples/blob/master/python_examples/GUIDE.md).

## Interface pair correlation function (grint)
Here we provide data suitable to test the program `grint.f90`,
which is available in the [Examples repository](https://github.com/Allen-Tildesley/examples).
The file `grint_data.zip` contains
a set of 100 configurations from a simulation of
a system of _N_=10000 atoms, interacting through
the Lennard-Jones potential cut (but not shifted) at _R_<sub>c</sub>=2.5&sigma;,
in a cubic box of side 30&sigma;, at a temperature _T_=0.90.
For this system, &rho;<sub>G</sub> &asymp; 0.024, &rho;<sub>L</sub> &asymp; 0.713.
Output files from `grint.f90` with default parameters are also provided.
The slices for _z_>0 (_z_<sub>1</sub> in the liquid) and
_c_<0 (_z_<sub>2</sub> further in the liquid) most resemble homogeneous liquid
pair distribution functions. Those with _z_<0, _c_>0, where both particles are
on the gas side, are the most noisy and show least structure.
For more details about the program,
refer to the [Fortran GUIDE](https://github.com/Allen-Tildesley/examples/blob/master/GUIDE.md).
