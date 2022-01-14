## bbhutil files

Among other things,
the `bbhutil` libraries contain utility functions for saving to `.sdf` files
(the basic file storage format used by `gh3d2m`).

See `INSTALL.md` in the main directory for some installation instructions.

You may also find this [webpage](http://laplace.physics.ubc.ca/Doc/rnpletal/)
from Matthew Choptuik's website to be helpful for installing this software
if you are running on a \*nix operating system.
Choptuik's website is much more complete than this README, so look there
if anything is not working!

From Choptuik's website, the general prerequisits are

* C compiler (gcc)
* Fortran 77 compiler (f77 or gfortran)
* perl
* flex and bison
* OpenGL headers: libmesagl1-devel
* OpenGL libraries

## Ubuntu installation notes from Luis Lehner (via Choptuik's website) 

The original link: [here](http://laplace.physics.ubc.ca/Doc/rnpletal/rnpletal-ubuntu.html)

```
sudo apt-get install gfortran
sudo apt-get install flex
sudo apt-get install bison
sudo apt-get install xutils-dev
sudo apt-get install mesa-common-dev
sudo apt-get install libglu1-mesa-dev
sudo apt-get install mesa-utils
sudo apt-get install libjpeg62
sudo apt-get install libjpeg62-dev
#sudo apt-get install libforms-dev
#sudo apt-get install libformsgl2
#sudo apt-get install libforms-bin
sudo apt-get install libxext-dev
sudo apt-get install libtiff-dev
sudo apt-get install libtiff-opengl
sudo apt-get install xfstt
sudo apt-get install t1-xfree86-nonfree
sudo apt-get install ttf-xfree86-nonfree
sudo apt-get install ttf-xfree86-nonfree-syriac
sudo apt-get install xfonts-75dpi
sudo apt-get install xfonts-100dpi
sudo apt-get install xfonts-100dpi-transcoded
sudo apt-get install xfonts-75dpi-transcoded
```

## Other misc. notes from Choptuik's website

If your machine has an NVidia card, 
and you have installed the proprietary driver, you should already have the needed libraries.
If not, install libmesagl1 Version 6.2 of the JPEG headers and libraries. 
IMPORTANT: mpeg\_encode (which is optional) will not compile / run with newer versions of the JPEG 
headers/libraries (version 8 in particular).  With luck your Linux distribution will have a separate version 6.2 package.
