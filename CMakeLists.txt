cmake_minimum_required(VERSION 3.15)

project(program)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

include(${CMAKE_SOURCE_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

add_executable(test_boost main_boost_test.cpp)
target_link_libraries(test_boost ${CONAN_LIBS})

add_executable(test_catch main_catch2.cpp)
target_link_libraries(test_catch ${CONAN_LIBS})

