cmake_minimum_required(VERSION 3.4)
project(kiss_fft LANGUAGES C)

add_library(${PROJECT_NAME
        include/kiss_fft/_kiss_fft_guts.h
        include/kiss_fft/kiss_fft.c
        include/kiss_fft/kiss_fft.h
        include/kiss_fft/tools/kiss_fftr.c
        include/kiss_fft/tools/kiss_fftr.h
)
target_include_directories(${PROJECT_NAME} PUBLIC include)
