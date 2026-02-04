cmake_minimum_required(VERSION 3.10)
project(PrintDriver)

add_executable(app
    src/main.cpp
)

add_executable(test_app
    test/test_main.cpp
)
