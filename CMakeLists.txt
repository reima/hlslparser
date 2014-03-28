cmake_minimum_required(VERSION 2.8)
project(hlslparser)

set(HEADERS
    src/CodeWriter.h
    src/Engine/Allocator.h
    src/Engine/Array.h
    src/Engine/Assert.h
    src/Engine/Log.h
    src/Engine/String.h
    src/Engine/StringPool.h
    src/GLSLGenerator.h
    src/HLSLGenerator.h
    src/HLSLParser.h
    src/HLSLTokenizer.h
    src/HLSLTree.h
)

set(SOURCES
    src/CodeWriter.cpp
    src/Engine/Log.cpp
    src/Engine/String.cpp
    src/Engine/StringPool.cpp
    src/GLSLGenerator.cpp
    src/HLSLGenerator.cpp
    src/HLSLParser.cpp
    src/HLSLTokenizer.cpp
    src/HLSLTree.cpp
    src/main.cpp
)

include_directories(src)

add_executable(hlslparser ${HEADERS} ${SOURCES})
