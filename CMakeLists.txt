cmake_minimum_required(VERSION 3.0.0)
project(SoundApp VERSION 0.1.0)

#include Help module with some custom helpful function
set(CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")
include(help)

make_sources(SRL_LIST)
add_executable(${PROJECT_NAME} ${SRL_LIST})