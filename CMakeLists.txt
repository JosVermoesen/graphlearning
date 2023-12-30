cmake_minimum_required(VERSION 3.13)

project(MY-RP6502-PROJECT C ASM)

add_subdirectory(tools)

add_executable(gdemo)
rp6502_executable(gdemo)
target_sources(gdemo PRIVATE
    src/bitmap_graphics.c
    src/main.c
)