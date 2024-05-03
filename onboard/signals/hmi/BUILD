load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "unreal_engine_request_proto",
    srcs = ["unreal_engine_request.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "unreal_engine_request_signal",
    proto = "unreal_engine_request_proto",
    proto_message_name = "moz_msg_UnrealEngineRequest",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "unreal_engine_status_response_proto",
    srcs = ["unreal_engine_status_response.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "unreal_engine_status_response_signal",
    proto = "unreal_engine_status_response_proto",
    proto_message_name = "moz_msg_UnrealEngineStatusResponse",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "service_mode_user_camera_input_proto",
    srcs = ["service_mode_user_camera_input.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "service_mode_user_camera_input_signal",
    proto = "service_mode_user_camera_input_proto",
    proto_message_name = "moz_msg_ServiceModeUserCameraInput",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "unreal_engine_heartbeat_stats_proto",
    srcs = ["unreal_engine_heartbeat_stats.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "unreal_engine_heartbeat_stats_signal",
    proto = "unreal_engine_heartbeat_stats_proto",
    proto_message_name = "moz_msg_UnrealEngineHeartbeatStats",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "unreal_engine_cluster_mode_request_proto",
    srcs = ["unreal_engine_cluster_mode_request.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "unreal_engine_cluster_mode_request_signal",
    proto = "unreal_engine_cluster_mode_request_proto",
    proto_message_name = "moz_msg_UnrealEngineClusterModeRequest",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "tell_tale_state_proto",
    srcs = ["tell_tale_state.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_nanopb = True,
)

mosaic_signal(
    name = "tell_tale_state_signal",
    proto = "tell_tale_state_proto",
    proto_message_name = "moz_msg_TellTaleState",
    visibility = ["//visibility:public"],
)
