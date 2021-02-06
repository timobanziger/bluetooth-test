cmake_minimum_required(VERSION 3.17)
project(untitled)

set(CMAKE_CXX_STANDARD 14)

include(FindBluetooth.cmake)

add_executable(bluetooth-test main.cpp)
target_link_libraries(bluetooth-test ${LIBBLUETOOTH_LIBRARIES})
