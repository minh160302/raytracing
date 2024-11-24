cmake_minimum_required(VERSION 3.13)  # CMake version check
project(raytracing)


# set(CMAKE_CXX_STANDARD 14)            # Enable c++14 standard

# Set to C++11
set ( CMAKE_CXX_STANDARD          11 )
set ( CMAKE_CXX_STANDARD_REQUIRED ON )
set ( CMAKE_CXX_EXTENSIONS        OFF )


set(SOURCE_FILES src/main.cpp)

include_directories(src)


# # Specific compiler flags below. We're not going to add options for all possible compilers, but if
# # you're new to CMake (like we are), the following may be a helpful example if you're using a
# # different compiler or want to set different compiler options.

# message (STATUS "Compiler ID: " ${CMAKE_CXX_COMPILER_ID})
# message (STATUS "Release flags: " ${CMAKE_CXX_FLAGS_RELEASE})
# message (STATUS "Debug flags: " ${CMAKE_CXX_FLAGS_DEBUG})


# Add executable target with source files listed in SOURCE_FILES variable
add_executable(raytracing ${SOURCE_FILES})