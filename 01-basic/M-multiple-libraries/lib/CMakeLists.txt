cmake_minimum_required(VERSION 3.5)

project(hello_external)

############################################################
# Create a library
############################################################

#Generate the static library from the library sources
add_library(hello_external STATIC 
    Hello.cpp
)

target_include_directories(hello_external
    PUBLIC 
        ${PROJECT_SOURCE_DIR}
)
