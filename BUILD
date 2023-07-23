# Description:
#   bzip2 is a high-quality data compressor.

load("@bazel_skylib//lib:selects.bzl", "selects")

licenses(["notice"])  # BSD derivative

alias(
    name = "bz2lib",
    actual = ":libbzip2",
    visibility = ["//visibility:public"],
)

alias(
    name = "libbzip2",
    actual = selects.with_or({
        ("@platforms//os:osx", "@platforms//os:ios", "@platforms//os:watchos", "@platforms//os:tvos"): ":bz2lib_system",
        "//conditions:default": ":bz2lib_source",
    }),
    visibility = ["//visibility:public"],
)

cc_library(
    name = "bz2lib_source",
    srcs = [
        "blocksort.c",
        "bz_version.h",
        "bzlib.c",
        "bzlib_private.h",
        "compress.c",
        "crctable.c",
        "decompress.c",
        "huffman.c",
        "randtable.c",
    ],
    hdrs = [
        "bzlib.h",
    ],
    copts = [
        "-O3",
        "-g",
    ],
)

cc_binary(
    name = "bzip2",
    srcs = [
        "bzip2.c",
    ],
    local_defines = [
        "BZ_UNIX",
    ],
    deps = [
        "libbzip2",
    ],
)

cc_library(
    name = "bz2lib_system",
    linkopts = ["-lbz2"],
)
