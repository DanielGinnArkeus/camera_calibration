cmake_minimum_required(VERSION 3.5.0)
project(MyOpenCVProject VERSION 0.1.0 LANGUAGES C CXX)
find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
include(CTest)
enable_testing()

add_executable(MyOpenCVProject src/main.cpp)
target_link_libraries( MyOpenCVProject ${OpenCV_LIBS} )

set_property(TARGET MyOpenCVProject PROPERTY CXX_STANDARD 17)