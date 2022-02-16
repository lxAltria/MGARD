cmake_minimum_required(VERSION 3.19)

project(mgard_progressive CXX C)
find_package(mgard)

add_executable (test_refactor test_refactor.cpp)
target_link_libraries(test_refactor mgard::mgard)

add_executable (test_reconstructor test_reconstructor.cpp)
target_link_libraries(test_reconstructor mgard::mgard)
