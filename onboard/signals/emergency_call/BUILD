load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "ecall_proto",
    srcs = ["ecall.proto"],
    visibility = ["//visibility:public"],
    with_java = True,
    with_nanopb = True,
    with_py = True,
    deps = [
    ],
)

mosaic_signal(
    name = "ecall_start_signal",
    proto = "ecall_proto",
    proto_message_name = "moz_msg_StartEmergencyCall",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "ecall_stop_signal",
    proto = "ecall_proto",
    proto_message_name = "moz_msg_EndEmergencyCall",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "ecall_sms_signal",
    proto = "ecall_proto",
    proto_message_name = "moz_msg_SendEmergencySMS",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "ecall_status_signal",
    proto = "ecall_proto",
    proto_message_name = "moz_msg_EmergencyCallState",
    visibility = ["//visibility:public"],
)
