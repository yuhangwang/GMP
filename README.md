# GMP
The GNU Multiple Precision Arithmetic Library

This is an unofficial redistribution of the binary&source form of the GNU GMP library (which is required  to compile programs like GCC), under the terms of LGPL v3 and GPL v2.

Please visit the official website for more details: https://gmplib.org/

Compilation note:
wget ftp://gcc.gnu.org/pub/gcc/infrastructure/gmp-4.3.2.tar.bz2
bunzip2 gmp-4.3.2.tar.bz2
tar xvf gmp-4.3.2.tar
mkdir build_gmp-4.3.2
cd build_gmp-4.3.2
../gmp-4.3.2/configure --prefix=/home/steven/local
make -j10
make check
make install


See the CheckResults.txt for partial output of "make check".
