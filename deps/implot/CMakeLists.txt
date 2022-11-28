cmake_minimum_required(VERSION 3.0)

project(implot)

SET(IMPLOT_SOURCES
    implot/implot.h 
    implot/implot_internal.h
    implot/implot.cpp
    implot/implot_items.cpp)
add_library(implot STATIC ${IMPLOT_SOURCES})
target_link_libraries(implot PUBLIC imgui)
target_include_directories(implot PUBLIC implot/)