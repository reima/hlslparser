cmake_minimum_required(VERSION 2.8)
project(hlslparser)

set(HEADERS
    src/CodeWriter.h
    src/GLSLGenerator.h
    src/HLSLGenerator.h
    src/HLSLParser.h
    src/HLSLTokenizer.h
    src/HLSLTree.h
)

set(SOURCES
    src/CodeWriter.cpp
    src/GLSLGenerator.cpp
    src/HLSLGenerator.cpp
    src/HLSLParser.cpp
    src/HLSLTokenizer.cpp
    src/HLSLTree.cpp
)

add_library(hlslparser ${HEADERS} ${SOURCES})
