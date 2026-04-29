cmake_minimum_required(VERSION 3.15)
project(smoke_test LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(smoke main.cpp)

enable_testing()
add_test(NAME smoke_test COMMAND smoke)
