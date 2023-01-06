cmake_minimum_required(VERSION 3.20)
project(libtorrent-demo)

set(CMAKE_CXX_STANDARD 17)
#add_definitions("-std=c++11")

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CMAKE_BUILD_TYPE "Release")

# 添加这两行
include(./conanbuildinfo.cmake)
conan_basic_setup()

include_directories(${CONAN_INCLUDE_DIRS})
link_directories(${CONAN_LIB_DIRS})

ADD_SUBDIRECTORY(src bin)