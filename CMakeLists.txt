### Basic settings
cmake_minimum_required (VERSION 2.6)

### Define the project
project (quadpack)
enable_language(Fortran)

### Set compiler flags
set(CMAKE_Fortran_MODULE_DIRECTORY ./OBJS)

### Define executable
add_library(quadpack
  quadpack.f90
)
