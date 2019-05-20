cmake_minimum_required(VERSION 3.5.0)
project(phonetisaurus)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fPIC")

set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)

add_library(phonetisaurus STATIC src/lib/util.cc)
target_include_directories(phonetisaurus PUBLIC src/include src src/3rdparty/utfcpp)