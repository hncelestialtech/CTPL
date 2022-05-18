cmake_minimum_required(VERSION 3.12)
project(ctpl_lib)

file(GLOB HEADERS "*.h")
#file(GLOB SOURCES "*.cc")
add_library(ctpl_lib ${HEADERS})

set_target_properties(ctpl_lib PROPERTIES LINKER_LANGUAGE CXX)

target_include_directories(ctpl_lib PUBLIC "..")