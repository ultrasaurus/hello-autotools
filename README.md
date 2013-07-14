# Understanding Autotools

http://www.lrde.epita.fr/~adl/dl/autotools.pdf
starting at page 97

Created src/main.c -- simple hello world program

Created based on tutorial:
* Makefile.am
* configure.ac
* src/Makefile.am


```
autoreconf --install
```

generates lots of files

### configuration templates
* Makefile.in
* src/Makefile.in
* config.h.in
* configure

### macro definitions
We used these 3rd party macros when we wrote configure.ac earlier
* aclocal.m4

### auxiliary build tools
* depcomp
* install-sh
* missing

### autotools cache files
* autom4te.cache/

## Build instructions
```
cd hello
./configure
make
make install
```

### OR even better
keep all the interim build files in their own directory
```
cd hello
mkdir build 
cd build
../configure
make
make install
```

## Run the program
$ hello
Hello World!
This is hello 0.1.


