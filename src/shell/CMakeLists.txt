cmake_minimum_required(VERSION 3.14)

project(shell)

add_library(${PROJECT_NAME} STATIC)

target_sources(${PROJECT_NAME} PRIVATE
    shell.hpp shell.cpp
)

target_include_directories(${PROJECT_NAME}
    INTERFACE ${CMAKE_SOURCE_DIR}/src/
)

target_include_directories(${PROJECT_NAME}
    PRIVATE ${CMAKE_SOURCE_DIR}/src/${PROJECT_NAME}
)
