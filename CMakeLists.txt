cmake_minimum_required(VERSION 3.16.3)
project(blif2bench VERSION 0.1)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(SOURCES
    src/Blif2bench.cpp
    src/Log.cpp
    src/Blifparse.cpp
    src/Str_cond.cpp
    src/Bliffile.cpp
)
add_executable(${PROJECT_NAME} ${SOURCES})

target_include_directories(${PROJECT_NAME}
    PRIVATE include/
)