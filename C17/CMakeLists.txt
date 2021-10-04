cmake_minimum_required(VERSION 3.10)
project(C17 LANGUAGES C VERSION 0.0.1)

set(CMAKE_C_STANDARD 17)

add_library(C17 include/unistl/string.h src/unistl/string.c)
