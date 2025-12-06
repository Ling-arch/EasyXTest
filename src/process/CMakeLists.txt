aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR} ProcessSrc)

add_library(Process SHARED ${ProcessSrc})

target_include_directories(Process
    PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}
)

target_link_libraries(Process
    PUBLIC PNCMap
)


