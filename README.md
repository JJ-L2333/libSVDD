# libSVDD: A Library for Support Vector Data Description
Copyright, 2020 Sohail R. Reddy  (sredd001@fiu.edu)

## Version v1.0.0


libSVDD is a library for single and multi-class classification written in object oriented Fortran 90 with a Python API. The library contains the following kernels:

* (1) Gaussian kernel: k(x,y) = exp(-(norm(x-y)/s)^2)
* (2) Exponential kernel: k(x,y) = exp(-(norm(x-y))/s^2)
* (3) Linear kernel: k(x,y) = x'*y
* (4) Laplace kernel: k(x,y) = exp(-(norm(x-y))/s)
* (5) Sigmoid kernel: k(x,y) = tanh(g*x'*y+c)
* (6) Polynomial kernel: k(x,y) = (x'*y+c)^d


<img src="/images/Training.png" width="400">             <img src="/images/Testing.png" width="400">


## Getting Started

The repository contains two options for using libSVDD. 

* Incorporating the libSVDD source code into your own code
* Linking directly with the static or shared libSVDD library (.so or .a) either using Fortran, C or Python (API)


### Prerequisites

Compiling the library requires the gfortran compiler. The Python API requires that numpy be installed


### Installing

Navigate to the source (src) directory and run the make command

```
cd src/; make
```

### Using libSVDD

The 'examples' folder contains two examples for using libSVDD in a Fortran and Python environment. The 'libSVDD.pdf' in the 'docs/' folder contains the theory and information on the use of libSVDD.


## How to Cite

If you use libSVDD, please cite the following 
```
Sohail R. Reddy, "libSVDD: A Library for Support Vector Data Description," 2020, DOI:10.5281/zenodo.3712443
```


## Contributing

The libSVDD framework can be expanded to allow for shared and distributed memory parallelization and for use on GPUs. Other areas include better solvers for the constrained optimization problems. Feel free to modify the library. The modification must conform to the GNU License Agreement


## Authors

**Sohail R. Reddy**


## License
This project is licensed under the GNU General Public License v2.0 - see the [LICENSE](LICENSE) file for details
