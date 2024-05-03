load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "gaming_controls_proto",
    srcs = ["gaming_controls.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "gaming_controls_signal",
    proto = "gaming_controls_proto",
    proto_message_name = "moz_msg_GamingControls",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "game_state_proto",
    srcs = ["game_state.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "game_state_signal",
    proto = "game_state_proto",
    proto_message_name = "moz_msg_GameState",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "remote_navigation_proto",
    srcs = ["remote_navigation.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "remote_navigation_signal",
    proto = "remote_navigation_proto",
    proto_message_name = "moz_msg_RemoteNavigation",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "media_metadata_proto",
    srcs = ["media_metadata.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "android_cluster_state_change_request_proto",
    srcs = ["android_cluster_state_change_request.proto"],
    visibility = ["//visibility:public"],
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "media_metadata_signal",
    proto = "media_metadata_proto",
    proto_message_name = "moz_msg_MediaMetadata",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "android_navigation_state_proto",
    srcs = ["android_navigation_state.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "android_navigation_state_signal",
    proto = "android_navigation_state_proto",
    proto_message_name = "moz_msg_AndroidNavigationState",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "carplay_user_request_proto",
    srcs = ["carplay_user_request.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "carplay_user_request_signal",
    proto = "carplay_user_request_proto",
    proto_message_name = "moz_msg_CarPlayUserRequest",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "carplay_ic_request_proto",
    srcs = ["carplay_ic_request.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "carplay_ic_request_signal",
    proto = "carplay_ic_request_proto",
    proto_message_name = "moz_msg_CarPlayICRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "android_cluster_state_change_request_signal",
    proto = "android_cluster_state_change_request_proto",
    proto_message_name = "moz_msg_AndroidClusterStateChangeRequest",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "android_vehicle_config_proto",
    srcs = ["android_vehicle_config.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    visibility = ["//visibility:public"],
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "android_vehicle_config_request_signal",
    proto = "android_vehicle_config_proto",
    proto_message_name = "moz_msg_AndroidVehicleConfigRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "android_vehicle_config_response_signal",
    proto = "android_vehicle_config_proto",
    proto_message_name = "moz_msg_AndroidVehicleConfigResponse",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "navigation_trip_info_proto",
    srcs = ["navigation_trip_info.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "navigation_trip_info_signal",
    proto = "navigation_trip_info_proto",
    proto_message_name = "moz_msg_NavigationTripInfo",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "android_process_info_proto",
    srcs = ["android_process_info.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "android_process_info_request_signal",
    proto = "android_process_info_proto",
    proto_message_name = "moz_msg_AndroidProcessInfoRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "android_process_info_response_signal",
    proto = "android_process_info_proto",
    proto_message_name = "moz_msg_AndroidProcessInfoResponse",
    visibility = ["//visibility:public"],
)
