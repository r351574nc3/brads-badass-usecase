load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")
load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")

git_repository(
    name = "com_github_r351574nc3_rules_canary",
    remote = "https://github.com/r351574nc3/brads-badass-canary.git",
    commit = "4ea7b8257d11ac33eef7e9daadbedbfe375d9236", # release 0.2.0
    shallow_since = "1543532884 -0500",
)

load("@com_github_r351574nc3_rules_canary//canary:canary.bzl", "canary_rules_dependencies")

canary_rules_dependencies()
