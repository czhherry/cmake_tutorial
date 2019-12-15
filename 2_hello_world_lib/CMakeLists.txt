cmake_minimum_required(VERSION 3.5)
project(say_hello_lib VERSION 1.0.0)

add_library(say-hello say_hello.cpp say_hello.h)

add_executable(hello main.cpp say_hello.cpp)

target_link_libraries(hello PRIVATE say-hello)