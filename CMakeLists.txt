cmake_minimum_required(VERSION 2.6)

project(travis_ci_test)

find_package(PythonInterp ${PY_VERSION})
find_package(PythonLibs REQUIRED)
if (PYTHONLIBS_FOUND)
    message(${PYTHON_INCLUDE_DIRS})
endif ()
