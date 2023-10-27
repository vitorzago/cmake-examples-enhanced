cmake_minimum_required(VERSION 3.5)

project(hello_binary)

############################################################
# Create an executable
############################################################

# Add an executable with the above sources
add_executable(hello_binary 
    main.cpp
)

# link the new hello_library target with the hello_binary target
target_link_libraries(hello_binary
    PRIVATE 
        hello_external
)
