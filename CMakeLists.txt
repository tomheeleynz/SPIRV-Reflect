cmake_minimum_required(VERSION 3.17)
project(SPIRV-REFLECT)

file(GLOB SRC_FILES "spirv_reflect.c" "spirv_reflect.h")

add_library(${PROJECT_NAME} STATIC ${SRC_FILES})
target_include_directories(${PROJECT_NAME} PUBLIC ".")