cmake_minimum_required(VERSION 3.0)

project(CannyDemo)

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS} ${PROJECT_SOURCE_DIR})

add_executable(edge edge.cpp)

target_link_libraries(edge ${OpenCV_LIBS})