cmake_minimum_required (VERSION 2.6)

project(brotli)

include_directories(include/ enc/ dec/)

add_executable(bro tools/bro.c 
common/dictionary.c
dec/bit_reader.c
dec/decode.c
dec/huffman.c
dec/state.c
enc/backward_references.c
enc/bit_cost.c
enc/block_splitter.c
enc/brotli_bit_stream.c
enc/cluster.c
enc/compress_fragment.c
enc/compress_fragment_two_pass.c
enc/encode.c
enc/entropy_encode.c
enc/histogram.c
enc/literal_cost.c
enc/memory.c
enc/metablock.c
enc/static_dict.c
enc/utf8_util.c
)
