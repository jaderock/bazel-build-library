package(default_visibility = ["//visibility:public"])

load("@rules_cc//cc:defs.bzl", "cc_library")

cc_library(
    name = "glfw-static",
    includes = ["include",],
    srcs = [
        "lib-vc2022/glfw3.lib",
    ],
    target_compatible_with = [
        "@platforms//cpu:x86_64",
        "@platforms//os:windows",
    ],
)

#    ["include/GLFW/glfw3.h",
    #    "include/GLFW/glfw3native.h",
    #],