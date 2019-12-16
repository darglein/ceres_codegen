cmake_minimum_required(VERSION 3.8 FATAL_ERROR)

project (codegen_helloworld VERSION 1.0.0 LANGUAGES CXX)

find_package(Ceres REQUIRED)


ceres_cost_functor(
    NAME SquareFunctor
    INPUT_FILE ${CMAKE_CURRENT_SOURCE_DIR}/square_functor.h
    )

add_executable(codegen_helloworld helloworld_codegen.cc )
target_link_libraries(codegen_helloworld ceres SquareFunctor)


