cmake_minimum_required(VERSION 3.5)

project(Log)

set(SRCS src/Log.cpp)
set(INCS include)
set(CMAKE_CXX_FLAGS -Wall)

include_directories(${INCS})

add_library(${PROJECT_NAME} ${SRCS})
