cmake_minimum_required(VERSION 3.17)

project(zlib-minimal)

add_library(
        zlib-minimal
        adler32.c
        crc32.c
        deflate.c
        gzguts.h
        inffast.c
        inflate.c
        inftrees.c
        trees.c
        zpipe.c
        zutil.c
)

target_include_directories(zlib-minimal PUBLIC .)