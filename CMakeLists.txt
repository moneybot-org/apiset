cmake_minimum_required(VERSION 3.10)

set(CMAKE_C_STANDARD 11)

project(apiset)

add_library(${PROJECT_NAME}
    src/apiset.c
    src/nls.c
    src/resolve.c
    src/string.c
    )

target_include_directories(${PROJECT_NAME} PUBLIC include)