cmake_minimum_required(VERSION 3.10)

project(test)

set(CMAKE_CXX_STANDARD 11)

file(GLOB_RECURSE SOURCES ${CMAKE_SOURCE_DIR}/src/*.cpp)

#message("source is:", ${SOURCES}, ${CMAKE_SOURCE_DIR})

add_executable(${PROJECT_NAME} ${SOURCES})

target_include_directories(${PROJECT_NAME} PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})
