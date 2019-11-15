cmake_minimum_required (VERSION 2.8)

project (test)
add_compile_options(-std=c++11)
# 将本文件夹下的源文件添加到变量 SRC_LIST 中
aux_source_directory(. SRC_LIST)
set (CMAKE_CXX_FLAGS  "${CMAKE_CXX_FLAGS} -g")
# 使用变量 SRC_LIST 中的源文件
add_executable(main ${SRC_LIST})