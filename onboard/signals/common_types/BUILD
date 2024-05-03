load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "camera_proto",
    srcs = ["camera.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "vehicle_timestamp_proto",
    srcs = ["vehicle_timestamp.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_go = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "light_schedule_proto",
    srcs = ["light_schedule.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        ":vehicle_timestamp_proto",
    ],
)

mosaic_proto_library(
    name = "button_state_proto",
    srcs = ["button_state.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "occupancy_state_proto",
    srcs = ["occupancy_state.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "vehicle_state_proto",
    srcs = ["vehicle_state.proto"],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        ":transition_status_proto",
    ],
)

mosaic_proto_library(
    name = "transition_status_proto",
    srcs = [
        "transition_status.proto",
    ],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "vehicle_state_signal",
    proto = "vehicle_state_proto",
    proto_message_name = "moz_msg_VehicleState",
    sysml_ids = ["dd7a4d8f-f4ce-4a79-8cfc-e2215c41beb3"],
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "vehicle_state_debug_signal",
    proto = "vehicle_state_proto",
    proto_message_name = "moz_msg_VehicleState",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "si_units_proto",
    srcs = ["si_units.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_go = True,
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "sentry_state_signal",
    proto = "sentry_mode_state_proto",
    proto_message_name = "moz_msg_SentryModeState",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "sentry_mode_state_proto",
    srcs = ["sentry_mode_state.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "chunked_message_proto",
    srcs = ["chunked_message.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "baseline_request_signal",
    proto = "baseline_proto",
    proto_message_name = "moz_msg_BaselineMessageWrapper",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "baseline_response_signal",
    proto = "baseline_proto",
    proto_message_name = "moz_msg_BaselineMessageWrapper",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "baseline_proto",
    srcs = ["baseline.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "fw_version_signal",
    proto = "fw_version_proto",
    proto_message_name = "moz_msg_FwVersion",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "fw_version_proto",
    srcs = ["fw_version.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)
