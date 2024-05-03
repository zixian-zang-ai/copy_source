load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "thermal_management_proto",
    srcs = ["thermal_management.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_proto_library(
    name = "fan_state_proto",
    srcs = ["fan_state.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_signal(
    name = "tme_component_control_signal",
    proto = "thermal_management_proto",
    proto_message_name = "moz_msg_TmeComponentControl",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "tme_sensor_readings_signal",
    proto = "thermal_management_proto",
    proto_message_name = "moz_msg_TmeSensorReadings",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "fan_state_signal",
    proto = "fan_state_proto",
    proto_message_name = "moz_msg_FanCurrentState",
    visibility = ["//visibility:public"],
)
