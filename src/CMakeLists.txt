cmake_minimum_required (VERSION 2.6)

project (helloworld)
MESSAGE(STATUS "This is SOURCE dir: ${PROJECT_BINARY_DIR}")



SET(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin) 
SET(LIBRARY_OUTPUT_PATH ${PROJECT_BINARY_DIR}/lib)

add_subdirectory(share)
add_executable(hello test.cpp)
add_subdirectory(helloworld)

INCLUDE_DIRECTORIES(share)
TARGET_LINK_LIBRARIES(hello share)