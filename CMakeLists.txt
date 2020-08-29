cmake_minimum_required(VERSION 3.16)

include(cmake/VersionFromGit.cmake)
version_from_git(INCLUDE_HASH ON)

project(wine VERSION ${VERSION})

configure_file(include/config.h.in include/config.h)

include_directories(${PROJECT_BINARY_DIR}/include include)

add_subdirectory(loader)