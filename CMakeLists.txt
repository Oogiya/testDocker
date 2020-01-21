cmake_minimum_required (VERSION 3.5)

project (testDock)

set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Werror -std=c++1y")

file (GLOB sources src/*.cpp include/*.h)
file (GLOB test_sources src/*.cpp include/*.h test/*.cpp)

add_executable (testDock ${sources})
add_executable (test_testDock ${test_sources})
