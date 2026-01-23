# 1. 指定 CMake 最低版本要求
cmake_minimum_required(VERSION 3.10)

# 2. 定义项目名称
project(CppDemo)

# 3. 设置 C++ 标准 (比如用 C++11 或 C++14)
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# 4. 核心指令：告诉 CMake，我要用这几个源文件生成一个叫 my_app 的可执行程序
# 你完全不需要关心 .o 文件怎么生成，CMake 会全自动处理！
add_executable(my_app main.cpp MathUtils.cpp)
