cmake_minimum_required(VERSION 3.31)
project(rubiks_cube_solver)

set(CMAKE_CXX_STANDARD 20)

add_executable(rubiks_cube_solver main.cpp
        Model/RubiksCube.h
        Model/RubiksCube.cpp
        Model/RubiksCube1dArray.cpp
        Model/RubiksCube3dArray.cpp)
