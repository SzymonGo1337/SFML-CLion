cmake_minimum_required(VERSION 3.15)
project(SFML-CLion)

set(SFML_STATIC_LIBRARIES TRUE)
set(CMAKE_BUILD_TYPE Debug)
find_package(SFML 2 COMPONENTS graphics system window audio network REQUIRED)
add_executable(SFML-CLion main.cpp)
target_link_libraries(SFML-CLion sfml-graphics sfml-system sfml-window sfml-audio sfml-network)