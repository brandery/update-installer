project(bzip2)

cmake_minimum_required(VERSION 2.6)


set (SOURCES
 blocksort.c
 bzlib.c
 compress.c
 crctable.c
 decompress.c
 huffman.c
 randtable.c
)

set (HEADERS
 bzlib.h
 bzlib_private.h
 zip.h
 libbz2.def
)


add_library(bzip2
 ${SOURCES}
 ${HEADERS}
)



