# CMakeLists.txt
# Created     : 2026. 02. 05.
# Last updated: 2026. 02. 05.

cmake_minimum_required(VERSION 3.1)
project(opentcad)

set(CMAKE_CXX_STANDARD 11)

set(SRCS
	main.cc
)

add_executable(${PROJECT_NAME} ${SRCS})
