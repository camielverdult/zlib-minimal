cmake_minimum_required(VERSION 3.17)

project(zlib-minimal)

add_library(
        zlib-minimal
        adler32.c
        crc32.c
        deflate.c
        inflate.c
        inffast.c
        inftrees.c
        trees.c
        zpipe.c
        zutil.c
)