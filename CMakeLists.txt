cmake_minimum_required(VERSION 3.18.1)

# set project name
project("OpenGL")

find_package(OpenGL REQUIRED)
include_directories(${OPENGL_INCLUDE_DIRS})

target_link_libraries(OpenGL ${OPENGL_LIBRARIES})

# adding main executable
add_executable("Main" "main.cpp")
