cmake_minimum_required(VERSION 3.1)

project(CoolGame VERSION 1.0)

include_directories(../game/include)

set(CMAKE_MAKE_PROGRAM c:/GetGnuWin32/bin/make.exe FORCE)
set(PROJECT_SOURCE_DIR ../game/src)
set(PROJECT_BINARY_DIR ../game/bin)

set(SOURCES
	../game/src/main.cpp
    ../game/src/common/Game.cpp
    ../game/src/common/GameObject.cpp
)

add_executable(${PROJECT_NAME} ${SOURCES})

