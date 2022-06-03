cmake_minimum_required(VERSION 3.16.3)

project(graphFirst C CXX)

set(CMAKE_CXX_STANDARD 17)

add_executable(main main.cpp)

add_subdirectory(ListGraph)
add_subdirectory(MatrixGraph)
add_subdirectory(SetGraph)
add_subdirectory(ArcGraph)
target_link_libraries(main LINK_PUBLIC ListGraph MatrixGraph SetGraph ArcGraph)