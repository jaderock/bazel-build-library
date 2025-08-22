package(default_visibility = ["//visibility:public"])

load("@rules_cc//cc:defs.bzl", "cc_library", "objc_library")

cc_library(
    name = "glad-lib",
    srcs = [
        "src/glad.c",
    ],
    includes = ["include"],
    hdrs = glob(["include/**/*.h"]),
    linkstatic = 1,
)
