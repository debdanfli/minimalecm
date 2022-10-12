cmake_minimum_required(VERSION 3.16)

set(PROJECT "miniprojekt")

project(${PROJECT} VERSION 0.0.0 LANGUAGES CXX)

# Global CMake variables are set here
set(CMAKE_CXX_STANDARD          17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS        OFF)

# Project/Library Names
set(LIBRARY_NAME    "${PROJECT}_MyLib")
set(EXECUTABLE_NAME "${PROJECT}_Executable")

# Add libraries
add_subdirectory("src")

# Add executable
add_subdirectory("app")