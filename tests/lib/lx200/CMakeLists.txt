# Copyright (c) 2025, OpenAstroTech
# SPDX-License-Identifier: Apache-2.0

cmake_minimum_required(VERSION 3.20.0)
find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})
project(lx200_lib_test)

# Include the LX200 library test sources
target_sources(app PRIVATE 
    src/main.c
    src/test_coordinates.c
)
