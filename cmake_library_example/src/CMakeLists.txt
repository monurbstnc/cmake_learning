project(CMakeLibraryExample) # It should be the same as root project

add_library(adder adder.c)

target_include_directories(adder PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/../include)