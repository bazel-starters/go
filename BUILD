"""Targets in the repository root"""

# We prefer BUILD instead of BUILD.bazel
# gazelle:build_file_name BUILD

load("@gazelle//:def.bzl", "gazelle")

exports_files(
    [
    ],
    visibility = ["//:__subpackages__"],
)

# gazelle:prefix github.com/example/project

gazelle(
    name = "gazelle",
    env = {
        "ENABLE_LANGUAGES": ",".join([
            "starlark",
            "proto",
            "go",
        ]),
    },
    gazelle = "@multitool//tools/gazelle",
)
