cmake_minimum_required(VERSION 3.16)
project(SDL3_template_project C)

set(CMAKE_C_STANDARD 17)

# Find the SDL3 package
find_package(SDL3 REQUIRED)

# Add your executable target
add_executable(SDL3_template_project main.c)

# Link SDL3 to your project
target_link_libraries(SDL3_template_project PRIVATE SDL3::SDL3)