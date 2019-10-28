cmake_minimum_required(VERSION 3.15)

project(program)

include(${CMAKE_SOURCE_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

add_executable(program main.cpp)
target_link_libraries(program ${CONAN_LIBS})
