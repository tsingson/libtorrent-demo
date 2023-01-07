cmake_minimum_required(VERSION 3.20)
project(libtorrent-demo)


set(CMAKE_CXX_STANDARD 14)
add_definitions("-std=c++11")


set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CMAKE_BUILD_TYPE "Release")

# 添加这两行
include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()
#find_package(libtorrent CONFIG REQUIRED)

include_directories(${CONAN_INCLUDE_DIRS})
link_directories(${CONAN_LIB_DIRS})

add_subdirectory(src)
#include_directories(${CONAN_INCLUDE_DIRS})
#link_directories(${CONAN_LIB_DIRS})
#add_executable(bt_get
#        src/bt-get.cpp)
#target_link_libraries(bt_get ${CONAN_LIBS})
#add_executable(bt_get3
#        src/bt-get3.cpp)
#target_link_libraries(bt_get3 ${CONAN_LIBS})