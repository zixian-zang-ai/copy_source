load("//tools/build:protobuf.bzl", "mosaic_proto_library")

package(default_visibility = ["//visibility:public"])

mosaic_proto_library(
    name = "intent",
    srcs = ["intent.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    with_cc = True,
    with_java = True,
    with_nanopb = True,
    with_py = True,
    with_strict_linting = False,
)

mosaic_proto_library(
    name = "vehicle_campaign_status_proto",
    srcs = ["vehicle_campaign_status.proto"],
    well_known_proto_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
        "@com_google_protobuf//:timestamp_proto",
    ],
    with_cc = True,
    with_java = True,
    with_nanopb = True,
    with_py = True,
    with_strict_linting = False,
)
