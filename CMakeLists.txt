cmake_minimum_required(VERSION 3.10)
project(stb LANGUAGES C)
set(Stb_INCLUDE_DIR STRING ${CMAKE_CURRENT_SOURCE_DIR})

file(GLOB_RECURSE Stb_INCLUDES
        "*.h"
)

file(GLOB_RECURSE Stb_SOURCES
        "*.c"
)

add_library(stb STATIC ${Stb_INCLUDES} ${Stb_SOURCES})
