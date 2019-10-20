cmake_minimum_required(VERSION 3.0)

project(dear_imgui)

set(
    HEADERS

    src/imconfig.h 
    src/imgui_internal.h
    src/imgui.h
    src/imstb_rectpack.h
    src/imstb_textedit.h
    src/imstb_truetype.h
)

set(
    SOURCES

    src/imgui_demo.cpp
    src/imgui_draw.cpp
    src/imgui_widgets.cpp
    src/imgui.cpp
)

add_library(imgui ${HEADERS} ${SOURCES})

target_include_directories(imgui PUBLIC src/)
