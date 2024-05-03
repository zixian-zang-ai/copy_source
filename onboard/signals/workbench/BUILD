load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "screen_record_proto",
    srcs = ["screen_record.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "screen_record_signal",
    proto = "screen_record_proto",
    proto_message_name = "moz_msg_ScreenRecord",
    visibility = ["//visibility:public"],
)
