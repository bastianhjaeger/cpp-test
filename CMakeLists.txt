# CMakeLists.txt for Task System

cmake_minimum_required(VERSION 3.16) # Set minimum CMake version
project(TaskSystem)

# Specify the output directories
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/plugins)
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/plugins)

# Set RPATH configuration
set(CMAKE_INSTALL_RPATH "${CMAKE_INSTALL_PREFIX}/../plugins")
set(CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE)
set(CMAKE_BUILD_WITH_INSTALL_RPATH TRUE)
set(CMAKE_MACOSX_RPATH TRUE)

# Add subdirectories
add_subdirectory(taskcore)
add_subdirectory(taskextras)
add_subdirectory(app)