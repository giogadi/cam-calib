cmake_minimum_required(VERSION 2.8.9)

project(cam-calib)

find_package(OpenCV REQUIRED)

add_executable(cam-calib cam-calib.cxx)
add_executable(cam-test test.cxx)

target_link_libraries(cam-calib ${OpenCV_LIBS})
target_link_libraries(cam-test ${OpenCV_LIBS})
