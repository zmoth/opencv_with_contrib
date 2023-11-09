cmake_minimum_required(VERSION 3.25)

project(opencv_with_contrib)

set(OPENCV_EXTRA_MODULES_PATH "${CMAKE_CURRENT_SOURCE_DIR}/opencv_contrib/modules" CACHE STRING "OpenCV额外模块")
set(OPENCV_VS_VERSIONINFO_SKIP NOT ${MSVC} CACHE BOOL "Skip generating the vs_version.rc file")

add_subdirectory(opencv)
