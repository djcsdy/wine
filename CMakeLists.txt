cmake_minimum_required(VERSION 3.16)

include(cmake/VersionFromGit.cmake)
version_from_git(INCLUDE_HASH ON)

project(wine VERSION ${VERSION})