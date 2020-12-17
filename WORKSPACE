load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")
load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")

git_repository(
    name = "com_github_r351574nc3_rules_canary",
    remote = "https://github.com/r351574nc3/brads-badass-canary.git",
    commit = "ee8ad4d96665b2e2a12e96d102338a7d4e206bee", # release 0.2.0
    shallow_since = "1607848914 -0700"
)

load("@com_github_r351574nc3_rules_canary//canary:deps.bzl", "canary_rules_dependencies")

canary_rules_dependencies()

http_archive(
    name = "rules_python",
    url = "https://github.com/bazelbuild/rules_python/releases/download/0.1.0/rules_python-0.1.0.tar.gz",
    sha256 = "b6d46438523a3ec0f3cead544190ee13223a52f6a6765a29eae7b7cc24cc83a0",
)
load("@rules_python//python:pip.bzl", "pip_install")
pip_install(   # or pip3_import
    name = "canary_deps",
    requirements = "@com_github_r351574nc3_rules_canary//:requirements.txt",
)
