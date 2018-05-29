cmake_minimum_required (VERSION 2.6)

project (helloworld)
MESSAGE(STATUS "This is BINARY dir: "${helloworld_BINARY_DIR})
MESSAGE(STATUS "This is SOURCE dir: "${helloworld_SOURCE_DIR})

add_executable(helloworld helloworld.cpp)