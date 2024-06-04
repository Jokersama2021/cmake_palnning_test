cmake_minimum_required(VERSION 3.29.0)#cmake最小的版本
project(planning)#项目
set(CMAKE_CXX_STANDARD 17)#c++版本

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)#可执行文件生成的目录
aux_source_directory(. SRC_LISTS)#获取当前目录下所有的.cpp文件打包放入SRC_LIST这个变量里面
add_executable(planning_main ${SRC_LISTS})#依赖