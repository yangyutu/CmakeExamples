cmake_minimum_required (VERSION 2.6)
project (Tutorialex2)
set (CMAKE_CXX_FLAGS "-std=c++0x")
find_package(OpenGL REQUIRED)
#include_directories("include")
add_executable (ex2 hello.cpp)

set (CMAKE_CXX_LINK_EXECUTABLE "${CMAKE_CXX_LINK_EXECUTABLE} -lGL -lGLU -lglut")
FIND_LIBRARY(LEMON 
	NAMES lemon
	PATHS /usr/lib /usr/local/lib)

set (CMAKE_VERBOSE_MAKEFILE ON)

