cmake_minimum_required(VERSION 3.15)
project(cchip8)

set(CMAKE_CXX_STANDARD 14)

add_executable(cchip8 src/main.cpp src/CPU.cpp src/CPU.h src/RAM.cpp src/RAM.h src/IO.cpp src/IO.h)

INCLUDE_DIRECTORIES(${SDL2_INCLUDE_DIRS})
TARGET_LINK_LIBRARIES(cchip8 ${SDL2_LIBRARIES})
