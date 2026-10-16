cmake_minimum_required(VERSION 3.28)
project(malloc_count C)

add_library(malloc_count
    malloc_count.c
    stack_count.c
)

target_include_directories(malloc_count PUBLIC ${CMAKE_SOURCE_DIR})

target_link_libraries(malloc_count PRIVATE ${CMAKE_DL_LIBS})
