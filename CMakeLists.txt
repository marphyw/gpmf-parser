# CMakeLists.txt
cmake_minimum_required (VERSION 3.8.2)
project (gpmf-parser)

set(CMAKE_SUPPRESS_REGENERATION true)
set(CMAKE_CONFIGURATION_TYPES "Debug;Release")

file(GLOB SOURCES GPMF_parser.c "demo/*.c")

add_library(gpmf-parser SHARED GPMF_parser.c)

add_executable(gpmf-parser-demo ${SOURCES})
