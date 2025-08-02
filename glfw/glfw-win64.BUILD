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

cc_import(
    name = "glfw-dll-import",
    interface_library = "lib-vc2022/glfw3dll.lib",
    shared_library = "lib-vc2022/glfw3.dll",
)

cc_library(
    name = "glfw-dynamic",
    includes = ["include",],
    deps = [
        ":glfw-dll-import",
    ],
)