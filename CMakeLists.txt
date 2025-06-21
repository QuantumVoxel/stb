cmake_minimum_required(VERSION 3.10)
project(stb LANGUAGES C)
set(Stb_INCLUDE_DIR STRING ${CMAKE_CURRENT_SOURCE_DIR})

file(GLOB Stb_INCLUDES "stb/*.h")
file(GLOB Stb_SOURCES "stb/*.c")

add_library(stb STATIC ${Stb_INCLUDES} ${Stb_SOURCES})

target_include_directories(stb PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
