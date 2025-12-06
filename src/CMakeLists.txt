project(EasyXTestMain)

add_subdirectory(pnc_map)
add_subdirectory(process)

add_executable(${PROJECT_NAME} main.cpp)

target_include_directories(${PROJECT_NAME} PUBLIC ${ProcessDir} ${PNCMapDir})

target_link_libraries(${PROJECT_NAME} PUBLIC PNCMap Process)