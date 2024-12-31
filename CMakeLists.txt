cmake_minimum_required(VERSION 3.8)

file(GLOB_RECURSE SRC CMAKE_CONFIGURE_DEPENDS *.h)

add_library(stb INTERFACE {$SRC})
set_property(TARGET stb PROPERTY CXX_STANDARD 20)
