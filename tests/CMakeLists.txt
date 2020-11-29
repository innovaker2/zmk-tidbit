cmake_minimum_required(VERSION 3.13.1)

set(BOARD native_posix)
set(SHIELD zmk_module)

find_package(zmk REQUIRED HINTS ../../zmk)
find_package(Zephyr REQUIRED HINTS ../../zephyr)

project(NONE)

target_sources(app PRIVATE main.c)