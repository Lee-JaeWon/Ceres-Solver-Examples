cmake_minimum_required(VERSION 2.8)

project(curve_fitting)

find_package(Ceres REQUIRED)
include_directories(${CERES_INCLUDE_DIRS})

# curve_fitting
add_executable(curve_fitting curve_fitting.cc)
target_link_libraries(curve_fitting Ceres::ceres)
