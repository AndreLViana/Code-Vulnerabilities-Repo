cmake_minimum_required(VERSION 3.26)
project(Code_Vulnerabilities)

set(CMAKE_CXX_STANDARD 17)

add_executable(Code_Vulnerabilities Buffer-Overflow/main.cpp/Buffer-Overflow.cpp
        Null-Pointer-Deference/main.cpp/Null-Pointer-Deference.cpp
        Integer-Overflow/main.cpp/Integer-Overflow.cpp
        Format-String/main.cpp/Format-String.cpp)
