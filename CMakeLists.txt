cmake_minimum_required(VERSION 3.22)

project(MusicPlayer VERSION 1.0.0 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED on)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_HOME_DIRECTORY}/bin)





set(SOURCE_DIR ${CMAKE_SOURCE_DIR}/src)

include_directories(${SOURCE_DIR})

file(GLOB_RECURSE SOURCES
    ${SOURCE_DIR}/*.cpp
)


add_executable(MusicPlayer ${SOURCES})

