cmake_minimum_required(VERSION 2.8.11)

project(ImGui)

set(SRC_FILES ${SRC_FILES}
    	imconfig.h,
		imgui.h,
		imgui.cpp,
		imgui_draw.cpp,
		imgui_internal.h,
		imgui_widgets.cpp,
		imstb_rectpack.h,
		imstb_textedit.h,
		imstb_truetype.h,
		imgui_demo.cpp
)

add_library(ImGui ${SRC_FILES})
target_include_directories(ImGui PUBLIC ./)