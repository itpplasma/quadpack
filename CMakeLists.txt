### Basic settings
cmake_minimum_required (VERSION 3.10)

### Define the project
project (quadpack)
enable_language(Fortran)

### Set compiler flags
set(CMAKE_Fortran_MODULE_DIRECTORY ./OBJS)
set(CMAKE_Fortran_FLAGS "-O3")

### Define executable
add_library(quadpack STATIC
  quadpack.f90
)
