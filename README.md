# agusthesis

## info mengenai HPC

direktori untuk simpan data 1TB : /mgpfs/scratch/agus105

direktori untuk simpan program 20GB : /mgpfs/home/agus105

settingan awal masuk linux ada di file .bashrc

untuk liat module library perintahnya "module avail"

untuk liat module apa yang sudah aktif/belum di "module list"

untuk load module library "module load xxx"

untuk HPC menggunakan library dari intel 

compiler GNU(serial/parallel) (C:gcc/mpicc C++:g++/mpicxx fortran:gfortran/mpif90)
compiler intel(serial/parallel) (C:icc/mpiicc C++:icpc/mpiicpc fortran: ifort/mpiifort)



## Install ADCIRC SWAN

# posisi direktori di $home

## Download ADCIRC . Dokumentasi di https://wiki.adcirc.org/Main_Page

git clone https://github.com/adcirc/adcirc.git

cd adcirc

## install wgrib

git clone https://github.com/weathersource/wgrib2.git

cd wgrib2

ubah di makefile CC=icc 

make clean

make -j12

make install


## install datetime fortran

git clone https://github.com/wavebitscientific/datetime-fortran




Compile ADCIRC
