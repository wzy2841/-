#[[
    这是一个注释，井号加两个方括号
]]
cmake_minimum_required(VERSION 3.0) #指定使用的最低版本


project(test) #项目名称
set(SRC add.cpp sub.cpp main.cpp)
file(GLOB SRC ${CMAKE_CURRENT_SOURCE_DIR}/src/*.cpp)
set(EXECUTABLE_OUTPUT_PATH /home/wzy2841/study/) #可执行程序输出路径
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include) #头文件路径
#set(CMAKE_CXX_STANDARD 11)
add_executable(app ${SRC})