cmake_minimum_required(VERSION 2.6)

project(travis_ci_test)

find_package(PythonInterp)
message(${PYTHON_EXECUTABLE})

execute_process(
    COMMAND python -c "from distutils import sysconfig; print(sysconfig.get_python_inc())"
    OUTPUT_VARIABLE PYTHON_INCLUDE_DIRS
    )

# find_package(PythonLibs REQUIRED)
message(${PYTHON_INCLUDE_DIRS})
