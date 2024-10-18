cmake_minimum_required(VERSION 3.15.0 FATAL_ERROR)

project(lenovo_unlock_bios LANGUAGES CXX)

if(NOT WIN32)
message(FATAL_ERROR "This application is Windows only" )
endif()

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(unlock src/main.cpp)
