# Description:
#   Common functionality for TensorFlow tooling

licenses(["notice"])  # Apache 2.0

exports_files(["LICENSE"])

package(
    default_visibility = ["//tensorflow:__subpackages__"],
)

py_library(
    name = "traverse",
    srcs = ["traverse.py"],
    srcs_version = "PY2AND3",
)

py_test(
    name = "traverse_test",
    srcs = ["traverse_test.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":traverse",
        "//tensorflow/python:platform_test",
    ],
)

filegroup(
    name = "all_files",
    srcs = glob(
        ["**/*"],
        exclude = [
            "**/METADATA",
            "**/OWNERS",
        ],
    ),
)
