


cmake_minimum_required(VERSION 3.30)

project(main)

add_library(a
 src/a.c
)


add_executable(main
 src/main.c)


target_link_libraries(main a)
target_include_directories(main PRIVATE include)


