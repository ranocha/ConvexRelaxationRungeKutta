# Relaxation Runge-Kutta Methods for Convex Functionals

[![License: MIT](https://img.shields.io/badge/License-MIT-success.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3066518.svg)](https://doi.org/10.5281/zenodo.3066518)

Relaxation Runge-Kutta methods are modifications of Runge-Kutta methods that
enforce conservation, dissipation, or other solution properties with respect
to any convex functional by the addition of a *relaxation parameter* that
multiplies the Runge-Kutta update at each time step.
Moreover, other desirable stability (such as strong stability preservation)
and efficiency (such as low storage requirements) properties are preserved.
The technique can be applied to both explicit and implicit Runge-Kutta
methods and requires only a small modification to existing implementations.
The computational cost at each step is the solution of one additional scalar
algebraic equation for which a good initial guess is available.

Relaxation Runge-Kutta methods for inner-product norms are developed and
studied in
```
@article{ketcheson2019relaxation,
  title={Relaxation {R}unge-{K}utta Methods: {C}onservation and
         Stability for Inner-Product Norms},
  author={Ketcheson, David I},
  journal={SIAM Journal on Numerical Analysis},
  volume={57},
  number={6},
  pages={2850--2870},
  year={2019},
  publisher={Society for Industrial and Applied Mathematics},
  doi={10.1137/19M1263662},
  eprint={1905.09847},
  eprinttype={arxiv},
  eprintclass={math.NA}
}
```
Generalizations to general functionals with a particular emphasis on convex ones
are developed and studied in the following article, which is available on
[arXiv.org](https://arxiv.org/abs/1905.09129).
```
@article{ranocha2020relaxation,
  title={Relaxation {R}unge-{K}utta Methods: Fully-Discrete Explicit
         Entropy-Stable Schemes for the Compressible {E}uler and
         {N}avier-{S}tokes Equations},
  author={Ranocha, Hendrik and Sayyari, Mohammed and Dalcin, Lisandro and
          Parsani, Matteo and Ketcheson, David I},
  journal={SIAM Journal on Scientific Computing},
  volume={42},
  number={2},
  pages={A612--A638},
  year={2020},
  month={03},
  publisher={Society for Industrial and Applied Mathematics},
  doi={10.1137/19M1263480},
  eprint={1905.09129},
  eprinttype={arxiv},
  eprintclass={math.NA}
}
```
Implementations of relaxation Ruge-Kutta methods and numerical experiments
reported in that article can be found in this repository. If you find these
schemes useful, please cite the articles mentioned above. If you use the
implementations provided here, please cite this repository as
```
@misc{ranocha2019relaxationRepository,
  title={{ConvexRelaxationRungeKutta}. {R}elaxation {R}unge--{K}utta
         Methods for Convex Functionals},
  author={Ranocha, Hendrik and Ketcheson, David I.},
  year={2019},
  month={05},
  howpublished={\url{https://github.com/ranocha/ConvexRelaxationRungeKutta}},
  doi={10.5281/zenodo.3066518}
}
```
Specialised implementations of relaxation Runge-Kutta methods for inner-product
norms are available at https://github.com/ketch/RRK_rr.


## Disclaimer

Everything is provided as is and without warranty. Use at your own risk!
