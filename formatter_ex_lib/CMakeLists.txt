cmake_minimum_required(VERSION 3.10)
project(formatter_ex)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CURRENT_SOURCE_DIR /Users/evgengrmit/Evgengrmit/workspace/projects/hw03)

add_library(formatter_ex STATIC ${CMAKE_CURRENT_SOURCE_DIR}/formatter_ex_lib/formatter_ex.cpp)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/formatter_ex_lib)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/formatter_lib)
target_link_libraries(formatter_ex formatter)
