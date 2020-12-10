cmake_minimum_required(VERSION 2.6)
project (lab2)

add_library(library STATIC calculator.h calculator.cpp)
add_executable(${PROJECT_NAME} main.cpp)

target_link_libraries(${PROJECT_NAME} library)
