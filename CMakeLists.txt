cmake_minimum_required(VERSION 3.0.0)
project(MyCMakeProject VERSION 0.1.0 LANGUAGES C CXX)

include(CTest)
enable_testing()

add_executable(MyCMakeProject src/main.cpp)

set_property(TARGET MyCMakeProject PROPERTY CXX_STANDARD 17)