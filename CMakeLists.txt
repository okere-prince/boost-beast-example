cmake_minimum_required(VERSION 3.0.0)
project(boostBeastTestApplication VERSION 0.1.0)

include(CTest)
enable_testing()

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup(TARGETS)

add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/httpserver)