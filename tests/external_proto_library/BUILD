package(default_visibility = ["//visibility:public"])

load("//cpp:rules.bzl", "cc_proto_library")
load("//java:rules.bzl", "java_proto_library")
load("//go:rules.bzl", "go_proto_library")

cc_proto_library(
    name = "cc_gapi",
    imports = [
        "external/com_github_googleapis_googleapis",
        #'external/com_github_google_protobuf/src',
    ],
    proto_deps = [
        "@com_github_googleapis_googleapis//:cc_label_proto",
    ],
    protos = ["message.proto"],
    verbose = 0,
)

java_proto_library(
    name = "java_gapi",
    imports = [
        "external/com_github_googleapis_googleapis",
        #'external/com_github_google_protobuf/src',
    ],
    proto_deps = [
        "@com_github_googleapis_googleapis//:java_label_proto",
    ],
    protos = ["message.proto"],
    # inputs = [
    #     "@com_github_googleapis_googleapis//:java_label_proto",
    #     "@com_github_google_protobuf//:well_known_protos"
    # ],
    verbose = 0,
)

go_proto_library(
    name = "go_gapi",
    imports = [
        "external/com_github_googleapis_googleapis",
        #'external/com_github_google_protobuf/src',
    ],
    inputs = [
        #"@com_github_googleapis_googleapis//:go_label_proto",
        #"@com_github_google_protobuf//:well_known_protos"
    ],
    proto_deps = [
        "@com_github_googleapis_googleapis//:go_label_proto",
    ],
    protos = ["message.proto"],
    verbose = 0,
)
