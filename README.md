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

They are developed and studied in the article
```
@article{ranocha2019relaxation,
  title={Relaxation {R}unge--{K}utta Methods: Fully-Discrete Explicit
         Entropy-Stable Schemes for the {E}uler and {N}avier--{S}tokes Equations},
  author={Ranocha, Hendrik and Sayyari, Mohammed and Dalcin, Lisandro and
          Parsani, Matteo and Ketcheson, David I.},
  year={2019},
  month={05},
  note={in preparation}
}
```
Implementations of relaxation Ruge-Kutta methods and numerical experiments
reported in that article can be found in this repository. If you find these
schemes useful, please cite the article mentioned above. If you use the
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


## Disclaimer

Everything is provided as is and without warranty. Use at your own risk!
