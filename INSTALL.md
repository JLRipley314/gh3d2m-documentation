## Installation/Dependencies

Generally, to run `gh3d2m` or its derivatives you'll need to install
(most of) the following libraries.

As a general rule, to compile `gh3d2m`, and many of the above libraries,
you wil need to copy the `Makefile.in.template` to your
own `Makefile.in` file, and then configure things manually within that file.

+ The `bbhutil` library (which is included in `bbhutil/rnpletal.tar.gz` in this repository),
  which is used by all the following dependencies.
  Some tips to installing rnpletal can be found 
  [here](http://laplace.physics.ubc.ca/Doc/rnpletal/) (see also the
  [UBC numerical relativity software webpage](http://laplace.physics.ubc.ca/Group/Software.html)).
  
  To install rnpletal from rnpletal.tar.gz file, move the file to, e.g. your home
  directory, unzip, and then install using the configuration file:
  ```
   tar zxf rnpletal.tar.gz
   cd rnpletal
   ./Install.gnu /usr/local  
  ```
  
+ The `PAMR` (Parallel Adaptive Mesh Refinment) library.
  Some old, unfinished documentation about this library can be found on the
  [UBC numerical relativity software webpage](http://laplace.physics.ubc.ca/Group/Software.html)
  A paper on the elliptic-hyperbolic solver can be found 
  [here, arXiv:gc-qc/0508110](https://arxiv.org/abs/gr-qc/0508110).
  A paper on the adaptations made for hydrodynamics by William East, Frans Pretorius, and
  Branson Stephens can be found [here, arXiv:1112.3094](https://arxiv.org/abs/1112.3094).
  Frans Pretorius PhD thesis also contains some description of this software, you can find
  his thesis [here](http://laplace.physics.ubc.ca/People/matt/Doc/Theses/). 

  Contact William East for a copy of the PAMR library source files. 

  This initial data solver also contains `idreader` software which allows for interfacing
  `TwoPunctures` initial data.
  Contact Will East for access to this code.

+ The `IDSolve` libraries. There are several libraries here, not all of which are
  necessary for running the code.
  To construct conformal thin-sandwhich initial
  data, the solver written by 
  [East et. al.](https://arxiv.org/abs/1208.3473) is containe dhere.
  This initial data solver also contains `idreader` software which allows for interfacing
  `TwoPunctures` initial data.
  Contact Will East for access to these libraries.

+ To construct Two-Puncture black hole initial data, use the 
  [c-interace to the twopunctures code](https://github.com/JLRipley314/Standalone-TwoPunctures-C-Cpp).
