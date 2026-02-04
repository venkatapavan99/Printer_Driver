cmake_minimum_required(VERSION 3.10)
project(CppJenkinsDemo)

set(CMAKE_CXX_STANDARD 11)

add_library(mathlib src/main.cpp)

add_executable(app src/main.cpp)
add_executable(test_app test/test_main.cpp)

target_link_libraries(test_app mathlib)
