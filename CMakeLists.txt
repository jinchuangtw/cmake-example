project(My_Project)

cmake_minimum_required(VERSION 2.8)

set(SOURCE_FILES src/main.cpp)

include_directories( src )
link_directories( src )
add_subdirectory( src )
add_executable( ${PROJECT_NAME} ${SOURCE_FILES} )
target_link_libraries( ${PROJECT_NAME} src )