cmake_minimum_required(VERSION 3.26.3)

project(hello_world LANGUAGES CXX)

add_executable(${PROJECT_NAME} main.cpp)

# message("PROJECT_NAME = ${PROJECT_NAME}")

function(print var)
    message(${var} = ${${var}})
endfunction()

print(PROJECT_NAME)