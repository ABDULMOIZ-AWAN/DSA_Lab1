cmake_minimum_required(VERSION 4.3)
project(DSA_Lab1)
cmake_minimum_required(VERSION 3.10)
project(DSA_Lab1)
set(CMAKE_CXX_STANDARD 17)

# Task 1: hello world
add_executable(hello hello.cpp)

# Task 2: utilities module + its smoke test
add_executable(test_utilities utilities.cpp test_utilities.cpp)
set(CMAKE_CXX_STANDARD 14)

include_directories(.)

add_executable(DSA_Lab1
        hello.cpp
        utilities.h
        utilities.cpp
        test_utilities.cpp)
