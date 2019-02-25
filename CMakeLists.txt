cmake_minimum_required(VERSION 3.13)
project(OpenGLTriangle)

set(CMAKE_CXX_STANDARD 14)
set(SOURCE_FILES glad.c main.cpp MyShaderLoader.h stb_image.cpp MyCamera.h)
add_executable(OpenGLTriangle ${SOURCE_FILES})
target_link_libraries(OpenGLTriangle GL GLU glfw3 X11 Xxf86vm Xrandr pthread Xi dl Xinerama Xcursor)