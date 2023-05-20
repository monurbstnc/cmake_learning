project(CMakeLibraryExample)

add_executable(main main.c)

target_link_libraries(main PRIVATE adder)