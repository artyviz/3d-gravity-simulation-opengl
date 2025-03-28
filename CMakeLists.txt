cmake_minimum_required(VERSION 3.10)
project(SpaceSimulation)
set(CMAKE_CXX_STANDARD 11)
set(GLFW_DIR "/path/to/glfw/lib/cmake")
find_package(GLFW REQUIRED)
find_package(GLEW REQUIRED)
find_package(glm REQUIRED)
set(IMGUI_SOURCES
    imgui/imgui.cpp
    imgui/imgui_demo.cpp
    imgui/imgui_draw.cpp
    imgui/imgui_tables.cpp
    imgui/imgui_widgets.cpp
    imgui/imgui_impl_glfw.cpp
    imgui/imgui_impl_opengl3.cpp
)
include_directories(${GLFW_INCLUDE_DIRS} ${GLEW_INCLUDE_DIRS} ${glm_INCLUDE_DIRS} ${CMAKE_CURRENT_SOURCE_DIR}/imgui)
set(SOURCE_FILES
    main.cpp
    ${IMGUI_SOURCES}
)
add_executable(SpaceSimulation ${SOURCE_FILES})
target_link_libraries(SpaceSimulation ${GLFW_LIBRARIES} ${GLEW_LIBRARIES} ${GLM_LIBRARIES})
