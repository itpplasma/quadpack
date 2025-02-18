### Basic settings
cmake_minimum_required (VERSION 3.10)

### Define the project
project (quadpack)
enable_language(Fortran)

### Define executable
add_library(quadpack STATIC
  quadpack.f90
)
