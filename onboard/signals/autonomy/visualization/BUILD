load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "color_proto",
    srcs = ["color.proto"],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "debug_message_proto",
    srcs = ["debug_message.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        ":color_proto",
    ],
)

mosaic_proto_library(
    name = "status_proto",
    srcs = ["status.proto"],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "vector3d_proto",
    srcs = ["vector3d.proto"],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_proto_library(
    name = "quaternion_proto",
    srcs = ["quaternion.proto"],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "size3d_proto",
    srcs = ["size3d.proto"],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_proto_library(
    name = "pose3d_proto",
    srcs = ["pose3d.proto"],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        ":quaternion_proto",
        ":vector3d_proto",
    ],
)

mosaic_proto_library(
    name = "navigation_waypoint_proto",
    srcs = ["navigation_waypoint.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "route_proto",
    srcs = ["route.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        ":navigation_waypoint_proto",
    ],
)

mosaic_proto_library(
    name = "agent_proto",
    srcs = ["agent.proto"],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        ":pose3d_proto",
        ":size3d_proto",
    ],
)

mosaic_proto_library(
    name = "detected_objects_proto",
    srcs = ["detected_objects.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        ":agent_proto",
        ":debug_message_proto",
        ":status_proto",
        "//onboard/signals/adas:image_and_detections_proto",
        "//onboard/signals/adas:traffic_light_state_proto",
    ],
)

mosaic_signal(
    name = "autonomy__visualization__detected_objects_signal",
    proto = "detected_objects_proto",
    proto_message_name = "moz_msg_DetectedObjects",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "localization_proto",
    srcs = ["localization.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        ":pose3d_proto",
        ":status_proto",
    ],
)

mosaic_signal(
    name = "autonomy__visualization__localization_signal",
    proto = "localization_proto",
    proto_message_name = "moz_msg_Localization",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "waypoint_proto",
    srcs = ["waypoint.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        ":pose3d_proto",
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_proto_library(
    name = "trajectory_proto",
    srcs = ["trajectory.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        ":waypoint_proto",
    ],
)

mosaic_proto_library(
    name = "planner_proto",
    srcs = ["planner.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        ":debug_message_proto",
        ":pose3d_proto",
        ":status_proto",
        ":trajectory_proto",
    ],
)

mosaic_signal(
    name = "autonomy__visualization__planner_signal",
    proto = "planner_proto",
    proto_message_name = "moz_msg_Planner",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "streams_status_proto",
    srcs = ["streams_status.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        ":status_proto",
        "//onboard/signals/common_types:si_units_proto",
        "//onboard/signals/common_types:vehicle_timestamp_proto",
    ],
)

mosaic_signal(
    name = "autonomy__visualization__streams_status_signal",
    proto = "streams_status_proto",
    proto_message_name = "moz_msg_StreamsStatus",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "hmi_navigation_proto",
    srcs = ["hmi_navigation.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        ":route_proto",
        ":status_proto",
    ],
)

mosaic_signal(
    name = "autonomy__visualization__navigation_signal",
    proto = "hmi_navigation_proto",
    proto_message_name = "moz_msg_Navigation",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "lane_info_proto",
    srcs = ["lane_info.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "autonomy__visualization__lane_info_signal",
    proto = "lane_info_proto",
    proto_message_name = "moz_msg_LaneInfo",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "speed_limit_proto",
    srcs = ["speed_limit.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_signal(
    name = "autonomy__visualization__speed_limit_signal",
    proto = "speed_limit_proto",
    proto_message_name = "moz_msg_SpeedLimit",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "lane_change_status_proto",
    srcs = ["lane_change_status.proto"],
    visibility = ["//visibility:public"],
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "autonomy__visualization__lane_change_status_signal",
    proto = "lane_change_status_proto",
    proto_message_name = "moz_msg_LaneChangeStatus",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "route_info_proto",
    srcs = ["route_info.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "autonomy__visualization__route_info_signal",
    proto = "route_info_proto",
    proto_message_name = "moz_msg_RouteInfo",
    visibility = ["//visibility:public"],
)
