cmake_minimum_required(VERSION 3.16)

project(libtest LANGUAGES CXX)

set(CMAKE_INCLUDE_CURRENT_DIR ON)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(libtest SHARED
  libtest_global.h
  libtest.cpp
  libtest.hpp
)

target_compile_definitions(libtest PRIVATE LIBTEST_LIBRARY)
