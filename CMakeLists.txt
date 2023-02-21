cmake_minimum_required(VERSION 3.22.0)

find_package(Zephyr)
project(pico_ice_zephyr)

target_sources(app PRIVATE src/main.c)
