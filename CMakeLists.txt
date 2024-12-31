cmake_minimum_required(VERSION 3.8)

file(GLOB STB_SRC CMAKE_CONFIGURE_DEPENDS *.h)

add_library(stb INTERFACE ${STB_SRC})
set_property(TARGET stb PROPERTY CXX_STANDARD 20)
target_include_directories(stb INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})
