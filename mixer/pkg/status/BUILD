package(default_visibility = ["//visibility:public"])

load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["status.go"],
    visibility = ["//visibility:public"],
    deps = [
        "@com_github_gogo_protobuf//proto:go_default_library",
        "@com_github_gogo_protobuf//types:go_default_library",
        "@com_github_hashicorp_go_multierror//:go_default_library",
        "@io_istio_api//mixer/v1:go_default_library",
        "@io_istio_gogo_genproto//googleapis/google/rpc:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    size = "small",
    srcs = ["status_test.go"],
    library = ":go_default_library",
    deps = [
        "@com_github_gogo_protobuf//proto:go_default_library",
        "@com_github_hashicorp_go_multierror//:go_default_library",
        "@io_istio_api//mixer/v1:go_default_library",
    ],
)
