## TO COMPILE

1. Navigate to program
2. sudo apt-get install libboost-all-dev
3. mkdir OutputLinux
4. cd OutputLinux
5. cmake . ..
6. make
7. Locate output binaries cmvs, genOption, and pmvs2 under OutpuxLinux/main

This is a modified version of CMVS/PMVS.

Main modification:
 - cross platform compilation Linux, Windows => CMake build system generator.
 - added bug fix from Nghia Ho.
 - make PLY, PSET, PATCH export faster and optional.
 - Replaced GSL simplex/lmfit with nlopt optimizer
 - Replaced image loading routines with CImg. Now PPMs are supported properly, with optional support for PNG and TIFF
 - Replaced BLAS/LAPACK with Eigen
 - Updated internal jpeg library and miniBoost
 - CMake-system now supports system boost, jpeg and other libraries if available. 
 - Replaced pthread with tinycthread to get rid of pthread.dll on Windows

Authors : 
[Original code author]  Yasutaka Furukawa http://www.cs.washington.edu/homes/furukawa/

[Initial Cmake multiplatform port ]	Pierre moulon pmoulon[AT]gmail.com

--------------------
- Web ressources : - 
--------------------
[CMVS/PMVS] http://http://grail.cs.washington.edu/software/cmvs/
[CMake version] http://opensourcephotogrammetry.blogspot.com/ https://github.com/pmoulon/CMVS-PMVS
