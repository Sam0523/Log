cmake_minimum_required(VERSION 3.5)

project(Log)

set(SRCS src/Log.cpp)
set(INCS include)

IF(MSVC)
	add_compile_options("/W3")
ELSE()
	add_compile_options("-Wall" "-Wextra")
ENDIF()


include_directories(${INCS})

add_library(${PROJECT_NAME} ${SRCS})
