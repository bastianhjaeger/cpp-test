cmake_minimum_required(VERSION 3.10)

project(CPP23_Task_Interface)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_subdirectory(core)
add_subdirectory(additional)
add_subdirectory(app)