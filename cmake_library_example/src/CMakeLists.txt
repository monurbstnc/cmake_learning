project(CMakeLibraryExample) # It should be the same as root project

add_library(adder adder.c)

target_include_directories(adder PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/../include)

# We use public publıc means that libraries are used by both target and any other targets that depends on it
#
#PRIVATE include directories are only used by the target itself. Sadece adder kullanacaksa PRVATE yapılabilir. 

#PUBLIC include directories are used by both the target and any other targets that depend on it.  

#INTERFACE include directories are used by other targets that depend on the target, but not by the target itself. 