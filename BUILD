"""Targets in the repository root"""

load("@gazelle//:def.bzl", "gazelle")

exports_files(
    [
    ],
    visibility = ["//:__subpackages__"],
)

# gazelle:prefix github.com/example/project

# We prefer BUILD instead of BUILD.bazel
# gazelle:build_file_name BUILD
# gazelle:exclude githooks/*

gazelle(
    name = "gazelle",
    env = {
        "ENABLE_LANGUAGES": ",".join([
            "starlark",
            "go",
        ]),
    },
    gazelle = "@multitool//tools/gazelle",
)
