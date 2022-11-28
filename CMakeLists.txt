cmake_minimum_required(VERSION 3.16.3)
project (log4fun)
set(CMAKE_CXX_STANDARD 11)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
add_library(log4fun SHARED src/main.cpp)
add_subdirectory(test/server-client-socket-comm/server)
add_subdirectory(test/server-client-socket-comm/client)
