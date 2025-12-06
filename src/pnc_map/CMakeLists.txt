# 设置库变量
aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR} PNCmapSrc)

add_library(PNCMap SHARED ${PNCmapSrc})

target_include_directories(PNCMap
    PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}
)

