cmake_minimum_required(VERSION 3.23)
project(Dodger)

set(CMAKE_CXX_STANDARD 20)
find_package(raylib 4.2 REQUIRED)
include_directories(/opt/homebrew/Cellar/raylib/4.2.0/include)
include_directories(/Music)
add_executable(Dodger main.cpp Player.h Window.h Racer.h Player.cpp Window.cpp Racer.cpp Drawing.cpp Logic.cpp Drawing.h Logic.h)
target_link_libraries(Dodger raylib)

