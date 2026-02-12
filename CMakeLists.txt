cmake_minimum_required(VERSION 3.20)

project(TaskSystem)

# Core library
add_subdirectory(taskcore)

# Extras
add_subdirectory(taskextras)

# Application
add_subdirectory(app)
