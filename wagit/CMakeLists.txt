cmake_minimum_required(VERSION 3.16)
project(wagit)

set(CMAKE_CXX_STANDARD 20)

add_executable(wagit main.cpp sources/WAGit.cpp headers/WAGit.h sources/Repository.cpp headers/Repository.h sources/GitObject.cpp headers/GitObject.h headers/GitConfig.h headers/GitExceptions.h sources/GitConfig.cpp includes/ini.h headers/Utils.h)

find_package(argh)
target_link_libraries(wagit argh)