cmake_minimum_required(VERSION 2.8.11)

project(ImGui)


add_library(ImGui 
		${PROJECT_SOURCE_DIR}/imconfig.h
		${PROJECT_SOURCE_DIR}/imgui.h
		${PROJECT_SOURCE_DIR}/imgui.cpp
		${PROJECT_SOURCE_DIR}/imgui_draw.cpp
		${PROJECT_SOURCE_DIR}/imgui_internal.h
		${PROJECT_SOURCE_DIR}/imgui_widgets.cpp
		${PROJECT_SOURCE_DIR}/imstb_rectpack.h
		${PROJECT_SOURCE_DIR}/imstb_textedit.h
		${PROJECT_SOURCE_DIR}/imstb_truetype.h
		${PROJECT_SOURCE_DIR}/imgui_demo.cpp	
)
target_include_directories(ImGui PUBLIC ./)