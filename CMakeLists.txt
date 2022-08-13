project(ImGuizmo LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)

add_library(ImGuizmo STATIC ImGuizmo.cpp ImSequencer.cpp ImCurveEdit.cpp ImGradient.cpp GraphEditor.cpp)

target_link_libraries(ImGuizmo PUBLIC IMGUI)
target_include_directories(ImGuizmo PUBLIC "../imgui/")