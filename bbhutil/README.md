## bbhutil files

Among other things,
the `bbhutil` libraries contain utility functions for saving to `.sdf` files
(the basic file storage format used by `gh3d2m`).

See `INSTALL.md` in the main directory for some installation instructions.

You may also find this [webpage](http://laplace.physics.ubc.ca/Doc/rnpletal/)
from Matthew Choptuik's website to be helpful for installing this software
if you are running on a \*nix operating system.

From Choptuik's website, the general prerequisits are

* C compiler (gcc)
* Fortran 77 compiler (f77 or gfortran)
* perl
* flex and bison
* OpenGL headers: libmesagl1-devel
* OpenGL libraries:

## Other notes (from Choptuik's website)

If your machine has an NVidia card, 
and you have installed the proprietary driver, you should already have the needed libraries.
If not, install libmesagl1 Version 6.2 of the JPEG headers and libraries. 
IMPORTANT: mpeg\_encode (which is optional) will not compile / run with newer versions of the JPEG 
headers/libraries (version 8 in particular).  With luck your Linux distribution will have a separate version 6.2 package.
