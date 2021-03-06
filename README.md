# GMP
**The GNU Multiple Precision Arithmetic Library**

This is an unofficial verbatim redistribution of the binary&source form of the GNU GMP library (a prerequisite for compiling programs like GCC), under the terms of LGPL 3.0 and GPL 2.0 licenses.

This redistribution is under the the same LGPL 3.0 and GPL 2.0 license.

Please visit the official website for more details: https://gmplib.org

## Usage
The binary/ folder contains both a tar.gz file and a folder, which are equivalent. You can use either one.

##Compilation notes

### Compilation environment
* CentOS 6.6
* x86_64 architecture
* Compiler: gcc version 4.4.7 20120313 (Red Hat 4.4.7-11)

### Compilation steps
#### Without C++ support
```bash
wget ftp://gcc.gnu.org/pub/gcc/infrastructure/gmp-4.3.2.tar.bz2
bunzip2 gmp-4.3.2.tar.bz2
tar xvf gmp-4.3.2.tar
mkdir build_gmp-4.3.2
cd build_gmp-4.3.2
../gmp-4.3.2/configure --prefix=/home/steven/install/libgmp/4.3.2
make -j10
make check
make install
```

#### With C++ support
```bash
wget ftp://gcc.gnu.org/pub/gcc/infrastructure/gmp-4.3.2.tar.bz2
bunzip2 gmp-4.3.2.tar.bz2
tar xvf gmp-4.3.2.tar
mkdir build_for_gcc-4.4.7_gmp-4.3.2
cd build_for_gcc-4.4.7_gmp-4.3.2
../gmp-4.3.2/configure --prefix=/home/steven/install/libgmp/with_cxx_support/for_gcc_4.4.7/4.3.2 --enable-cxx=yes
make -j10
make check
make install
```



### Quality verification
See the "QualityVerification.txt" for the output of "make check".
