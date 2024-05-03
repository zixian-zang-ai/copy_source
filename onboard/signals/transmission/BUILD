load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "drive_mode_proto",
    srcs = ["drive_mode.proto"],
    visibility = ["//visibility:public"],
    with_go = True,
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "drive_mode_signal",
    proto = "drive_mode_proto",
    proto_message_name = "moz_msg_DriveMode",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "drive_mode_to_light_manager_signal",
    proto = "drive_mode_proto",
    proto_message_name = "moz_msg_DriveMode",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "drive_mode_to_app_signal",
    proto = "drive_mode_proto",
    proto_message_name = "moz_msg_DriveMode",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "drive_mode_request_signal",
    proto = "drive_mode_proto",
    proto_message_name = "moz_msg_DriveModeRequest",
    visibility = ["//visibility:public"],
)
