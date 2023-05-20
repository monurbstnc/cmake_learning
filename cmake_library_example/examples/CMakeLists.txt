project(CMakeLibraryExample)

add_executable(main main.c)

target_link_libraries(main PRIVATE adder)

# I add PRIVATE so I want to use that library only main targer

#target_name is the name of the target to which the libraries will be linked.
#PRIVATE libraries are only used by the target itself.
#PUBLIC libraries are used by both the target and any other targets that depend on it.
#INTERFACE libraries are used by other targets that depend on the target, but not by the target itself.
#library_name1, library_name2, etc., are the names of the libraries to be linked.