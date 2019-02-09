#specify the minimum version for CMake

cmake_minimum_required(VERSION 2.8)

#project name
project(helloWorld)

#Set the output folder where your program will be created
set(CMAKE_BINARY_DIR ${CMAKE_SOURCE_DIR}/bin)
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_BINARY_DIR})

#Set include directory
include_directories("${PROJECT_SOURCE_DIR}")

#Now build source file
add_executable(helloWorld helloWorld.cpp)

