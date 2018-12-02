cmake_minimum_required(VERSION 3.0.0)
project(httpServer VERSION 0.1.0)

file (GLOB_RECURSE SOURCES "*.cpp")

add_executable(${PROJECT_NAME} ${SOURCES})
target_sources(${PROJECT_NAME} PRIVATE ${SOURCES})
target_link_libraries(${PROJECT_NAME} CONAN_PKG::boost_beast)
set_property(TARGET ${PROJECT_NAME} PROPERTY CXX_STANDARD 11)