cmake_minimum_required(VERSION 3.13)

include(pico-sdk/external/pico_sdk_import.cmake)

project(test)
pico_sdk_init()


add_executable(test
    test.c
)

target_link_libraries(test pico_stdlib pico_cyw43_arch_none)

pico_add_extra_outputs(test)
