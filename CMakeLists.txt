cmake_minimum_required(VERSION 2.6)

project(travis_ci_test)

find_package(PythonInterp)
message(${PYTHON_EXECUTABLE})

execute_process(
    COMMAND ${PYTHON_EXECUTABLE} -c "from distutils import sysconfig; print(sysconfig.get_python_inc())"
    OUTPUT_VARIABLE PYTHON_INCLUDE_DIRS)

message(${PYTHON_INCLUDE_DIRS})
