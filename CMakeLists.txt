cmake_minimum_required(VERSION 3.12.0)
project(EasyXTest
    VERSION 0.1.0
    DESCRIPTION "EasyX Test Project"
    HOMEPAGE_URL "https://github.com/Ling-arch/EasyXTest"
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON)

# 变量设置
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)

set(ProcessDir ${CMAKE_SOURCE_DIR}/src/process)
set(PNCMapDir ${CMAKE_SOURCE_DIR}/src/pnc_map)

# ADD_SUBDIRECTORY(src), has cmakeLists.txt directory all included
add_subdirectory(src)
