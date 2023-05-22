cmake_minimum_required(VERSION 3.15)

project(cmakewithtest)

add_subdirectory(include)
add_subdirectory(src)

option(BUILD_TESTS "" ON)

option(BUILD_EXAMPLES "" ON)

if(BUILD_TEST)
    message(STATUS "Building tests....")
    add_subdirectory(tests)
endif()

if(BUILD_EXAMPLES)
    message(STATUS "Building tests....")
    add_subdirectory(examples)
endif()