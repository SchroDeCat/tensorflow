# Description:
#   contains parts of TensorFlow that are experimental or unstable and which are not supported.

licenses(["notice"])  # Apache 2.0

exports_files(["LICENSE"])

package(default_visibility = ["//tensorflow:__subpackages__"])

py_library(
    name = "graph_editor_py",
    srcs = [
        "__init__.py",
        "edit.py",
        "match.py",
        "reroute.py",
        "select.py",
        "subgraph.py",
        "transform.py",
        "util.py",
    ],
    srcs_version = "PY2AND3",
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
    visibility = ["//tensorflow:__subpackages__"],
)

py_test(
    name = "util_test",
    srcs = ["tests/util_test.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":graph_editor_py",
        "//tensorflow:tensorflow_py",
        "//tensorflow/python:framework_test_lib",
        "//tensorflow/python:platform_test",
    ],
)

py_test(
    name = "select_test",
    srcs = ["tests/select_test.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":graph_editor_py",
        "//tensorflow:tensorflow_py",
        "//tensorflow/python:framework_test_lib",
        "//tensorflow/python:platform_test",
    ],
)

py_test(
    name = "match_test",
    srcs = ["tests/match_test.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":graph_editor_py",
        "//tensorflow:tensorflow_py",
        "//tensorflow/python:framework_test_lib",
        "//tensorflow/python:platform_test",
    ],
)

py_test(
    name = "subgraph_test",
    srcs = ["tests/subgraph_test.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":graph_editor_py",
        "//tensorflow:tensorflow_py",
        "//tensorflow/python:framework_test_lib",
        "//tensorflow/python:platform_test",
    ],
)

py_test(
    name = "reroute_test",
    srcs = ["tests/reroute_test.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":graph_editor_py",
        "//tensorflow:tensorflow_py",
        "//tensorflow/python:framework_test_lib",
        "//tensorflow/python:platform_test",
    ],
)

py_test(
    name = "edit_test",
    srcs = ["tests/edit_test.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":graph_editor_py",
        "//tensorflow:tensorflow_py",
        "//tensorflow/python:framework_test_lib",
        "//tensorflow/python:platform_test",
    ],
)

py_test(
    name = "transform_test",
    srcs = ["tests/transform_test.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":graph_editor_py",
        "//tensorflow:tensorflow_py",
        "//tensorflow/python:framework_test_lib",
        "//tensorflow/python:platform_test",
    ],
)
