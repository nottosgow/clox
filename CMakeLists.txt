cmake_minimum_required(VERSION 4.1.0)
project(clox C)

set (CMAKE_C_STANDARD 99)
set (CMAKE_C_STANDARD_REQUIRED True)

# Source files
set(SRC_FILES 
        ~/projects/clox/src/main.c
        ~/projects/clox/src/chunk.c
        ~/projects/clox/src/debug.c
        ~/projects/clox/src/value.c
        ~/projects/clox/src/memory.c

)

# Include directories
include_directories(
        ~/projects/clox/src
        ~/projects/clox/include
)

# Create executable
add_executable(clox_app ${SRC_FILES})

