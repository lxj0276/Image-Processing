cmake_minimum_required(VERSION 2.8)
project( week4 )
find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable( edge_detection ../src/edge_detection.cpp )
target_link_libraries( edge_detection ${OpenCV_LIBS} )
add_executable( filter ../src/filter.cpp )
target_link_libraries( filter ${OpenCV_LIBS} )
