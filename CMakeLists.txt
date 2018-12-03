cmake_minimum_required(VERSION 3.5)
project(matmul_demo C)

set(CMAKE_C_STANDARD 11)
set(CMAKE_C_FLAGS "-O0  -Wall")

add_executable(matmul_demo main.c utils.h matmul.c utils.c)
target_link_libraries(matmul_demo pthread)