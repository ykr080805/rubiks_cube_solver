cmake_minimum_required(VERSION 3.31)
project(rubiks_cube_solver)

set(CMAKE_CXX_STANDARD 20)

add_executable(rubiks_cube_solver main.cpp
        Model/RubiksCube.h
        Model/RubiksCube.cpp
        Model/RubiksCube1dArray.cpp
        Model/RubiksCube3dArray.cpp
        Model/RubiksCubeBitboard.cpp
        Solver/DFSSolver.h
        Solver/BFSSolver.h
        Solver/IDDFSSolver.h
        Solver/IDAstarSolver.h
        PatternDatabases/NibbleArray.h
        PatternDatabases/NibbleArray.cpp
        PatternDatabases/PatternDatabase.h
        PatternDatabases/PatternDatabase.cpp
        PatternDatabases/PermutationIndexer.h
        PatternDatabases/math.h
        PatternDatabases/math.cpp
        PatternDatabases/CornerPatternDatabase.h
        PatternDatabases/CornerPatternDatabase.cpp
        PatternDatabases/CornerDBMaker.h
        PatternDatabases/CornerDBMaker.cpp
        Model/PatternDatabase/PatternDatabase.h)
