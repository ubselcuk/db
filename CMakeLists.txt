cmake_minimum_required(VERSION 3.16.3)
project(db)

set(CMAKE_CXX_STANDARD 17)

find_package(Curses REQUIRED)
include_directories(${CURSES_INCLUDE_DIR})

add_executable(db main.cpp)
target_link_libraries(db ${CURSES_LIBRARIES})