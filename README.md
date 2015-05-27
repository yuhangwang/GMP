# GMP
**version: 4.3.2**

The GNU Multiple Precision Arithmetic Library

This is an unofficial distribution of the binary&source form of the GNU GMP library (a prerequisite for compiling programs like GCC), under the terms of LGPL v3 and GPL v2.

This distribution is under the the same LGPL v3 and GPL v2 license.

Please visit the official website for more details: https://gmplib.org/

##Compilation note:

### Compilation environment
* CentOS 6.6
* x86_64 architecture
* Compiler: gcc version 4.4.7 20120313 (Red Hat 4.4.7-11)

### Compilation steps
```bash
wget ftp://gcc.gnu.org/pub/gcc/infrastructure/gmp-4.3.2.tar.bz2
bunzip2 gmp-4.3.2.tar.bz2
tar xvf gmp-4.3.2.tar
mkdir build_gmp-4.3.2
cd build_gmp-4.3.2
../gmp-4.3.2/configure --prefix=/home/steven/local
make -j10
make check
make install
```

See the CheckResults.txt for partial output of "make check".
