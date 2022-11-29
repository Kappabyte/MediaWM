# MediaWM - a window manager for a media center computer

cmake_minimum_required(VERSION 3.6)

project(MediaWM)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

find_package(X11 REQUIRED)
link_libraries(${X11_LIBRARIES})
include_directories(${X11-INCLUDE_DIR})

set(SOURCE_FILES src/main.cpp)
add_executable(MediaWM ${SOURCE_FILES})
