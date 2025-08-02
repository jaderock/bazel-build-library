load("@rules_cc//cc:cc_binary.bzl", "cc_binary")

cc_binary(
    name = "glfw-window",
    srcs = [
        ":glfw-window.cc",
    ],
    deps = [
        "@glfw//:glfw",
    ],
)

cc_binary(
    name = "glfw-win64",
    srcs = [
        ":glfw-window.cc",
    ],
    linkopts = [
        "gdi32.lib",
        "shell32.lib",
        "user32.lib",
    ],
    deps = [
        "@glfw-prebuilt-win64//:glfw-static",
    ],
)

cc_binary(
    name = "glfw-win64-dll",
    srcs = [
        ":glfw-window.cc",
    ],
    linkopts = [
        "gdi32.lib",
        "shell32.lib",
        "user32.lib",
    ],
    deps = [
        "@glfw-prebuilt-win64//:glfw-dynamic",
    ],
)
