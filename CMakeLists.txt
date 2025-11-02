add_library(ymfm_for_pico INTERFACE)

target_sources(
    ymfm_for_pico
    INTERFACE
    ${CMAKE_CURRENT_LIST_DIR}/src/ymfm_adpcm.cpp
    ${CMAKE_CURRENT_LIST_DIR}/src/ymfm_misc.cpp
    ${CMAKE_CURRENT_LIST_DIR}/src/ymfm_opl.cpp
    ${CMAKE_CURRENT_LIST_DIR}/src/ymfm_opm.cpp
    ${CMAKE_CURRENT_LIST_DIR}/src/ymfm_opn.cpp
    ${CMAKE_CURRENT_LIST_DIR}/src/ymfm_opq.cpp
    ${CMAKE_CURRENT_LIST_DIR}/src/ymfm_opz.cpp
    ${CMAKE_CURRENT_LIST_DIR}/src/ymfm_pcm.cpp
    ${CMAKE_CURRENT_LIST_DIR}/src/ymfm_ssg.cpp
)

target_include_directories(ymfm_for_pico INTERFACE ${CMAKE_CURRENT_LIST_DIR}/src)

target_link_libraries(ymfm_for_pico INTERFACE pico_stdlib)
