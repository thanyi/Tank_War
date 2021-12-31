cmake_minimum_required(VERSION 3.20)
project(c_game3)

set(CMAKE_CXX_STANDARD 14)
#声明头文件路径
set(INC_DIR ./include)
#声明链接库路径
set(LINK_DIR ./lib)
#引入头文件
include_directories(${INC_DIR})
#引入库文件
link_directories(${LINK_DIR})
#设置要连接的库
link_libraries(easyXa)
link_libraries(easyXw)

add_executable(c_game3 main.cpp)
target_link_libraries(c_game3 easyXa)
target_link_libraries(c_game3 easyXw)



