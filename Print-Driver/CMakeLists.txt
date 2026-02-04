cmake_minimum_required(VERSION 3.10)
project(PrintDriver)

# Library – NO main()
add_library(mathlib
    src/mathlib.cpp
)

# App executable – has main()
add_executable(app
    src/main.cpp
)
target_link_libraries(app mathlib)

# Test executable – has its own main()
add_executable(test_app
    test/test_main.cpp
)
target_link_libraries(test_app mathlib)
