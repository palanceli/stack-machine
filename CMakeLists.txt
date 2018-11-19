cmake_minimum_required(VERSION 3.4.1)

PROJECT(stack_machine)

INCLUDE_DIRECTORIES(include)

set(CMAKE_BUILD_TYPE "Debug")

ADD_EXECUTABLE(smr instructions.cpp machine.cpp upper.cpp fileptr.cpp smr.cpp)
ADD_EXECUTABLE(smc instructions.cpp machine.cpp upper.cpp error.cpp fileptr.cpp parser.cpp compiler.cpp smc.cpp)
ADD_EXECUTABLE(smd instructions.cpp machine.cpp upper.cpp error.cpp fileptr.cpp smd.cpp)
ADD_EXECUTABLE(sm  instructions.cpp machine.cpp upper.cpp error.cpp fileptr.cpp  parser.cpp compiler.cpp sm.cpp)
