cmake_minimum_required(VERSION 3.26.4)

project(segger_rtt CXX C ASM)

add_library(segger_rtt RTT/SEGGER_RTT.c RTT/SEGGER_RTT_printf.c RTT/SEGGER_RTT_ASM_ARMv7M.S)
target_include_directories(segger_rtt PUBLIC RTT Config)