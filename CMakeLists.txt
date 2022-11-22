cmake_minimum_required(VERSION 3.17)

project(zlib-minimal)

add_library(
        zlib-minimal
        adler32.c
        crc32.c
        crc32.h
        deflate.c
        deflate.h
        gzguts.h
        inffast.c
        inffast.h
        inffixed.h
        inflate.c
        inflate.h
        inftrees.c
        inftrees.h
        trees.c
        trees.h
        zconf.h
        zlib.h
        zpipe.c
        zpipe.h
        zutil.c
        zutil.h
)