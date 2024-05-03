load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "screenshot_request_proto",
    srcs = ["screenshot_request.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "camera_viewer_screenshot_request_signal",
    proto = "screenshot_request_proto",
    proto_message_name = "moz_msg_ScreenshotRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "cluster_screenshot_request_signal",
    proto = "screenshot_request_proto",
    proto_message_name = "moz_msg_ScreenshotRequest",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "baseline_status_proto",
    srcs = ["baseline_status.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "baseline_status_signal",
    proto = "baseline_status_proto",
    proto_message_name = "moz_msg_BaselineStatus",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "baseline_command_proto",
    srcs = ["baseline_command.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_java = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        ":baseline_status_proto",
    ],
)

mosaic_signal(
    name = "baseline_command_signal",
    proto = "baseline_command_proto",
    proto_message_name = "moz_msg_BaselineCommand",
    visibility = ["//visibility:public"],
)
