cmake_minimum_required(VERSION 3.21)
project(TrojanAlpha)

find_package(OpenGl REQUIRED)

set(CMAKE_CXX_STANDARD 14)

include_directories(include)

link_directories(lib)

add_executable(TrojanAlpha main.cpp glad.c Shader.cpp Shader.h)

target_link_libraries(TrojanAlpha glfw3 opengl32)