cmake_minimum_required(VERSION 3.25)

project(microcpp)

set(SOURCE_FILES src/main.c)

include_directories("/usr/local/include" ${PROJECT_SOURCE_DIR}/src)

link_directories("/usr/local/lib")

include(cmake/CPM.cmake)

add_executable(microcpp ${SOURCE_FILES})
