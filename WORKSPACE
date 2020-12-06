load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")
load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")

git_repository(
    name = "com_github_r351574nc3_rules_canary",
    remote = "https://github.com/r351574nc3/brads-badass-canary.git",
    commit = "259dae1886da4444de54ed94dd761fd2cf3dbd39", # release 0.2.0
)

load("@com_github_r351574nc3_rules_canary//canary:deps.bzl", "canary_rules_dependencies")

canary_rules_dependencies()
