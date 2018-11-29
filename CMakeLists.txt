cmake_minimum_required(VERSION 2.6)

project(travis_ci_test)

find_package(PythonInterp)
message(${PYTHON_EXECUTABLE})

find_package(PythonLibs REQUIRED)
message(${PYTHON_INCLUDE_DIRS})
