load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "autonomy_navigation_proto",
    srcs = ["autonomy_navigation.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "autonomy__input__navigation_signal",
    proto = "autonomy_navigation_proto",
    proto_message_name = "moz_msg_AutonomyNavigation",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "user_voiceinput_proto",
    srcs = ["user_voiceinput.proto"],
    visibility = ["//visibility:public"],
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "autonomy__input__voiceinput_signal",
    proto = "user_voiceinput_proto",
    proto_message_name = "moz_msg_UserVoiceInput",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "autonomy_traffic_lights_info_proto",
    srcs = ["autonomy_traffic_lights_info.proto"],
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
    name = "autonomy__input__traffic_lights_info_signal",
    proto = "autonomy_traffic_lights_info_proto",
    proto_message_name = "moz_msg_AutonomyTrafficLightsInfo",
    visibility = ["//visibility:public"],
)

# Additional GPS signal to track the vehicle controller's GPS position.
# This is different from gps_position_signal since this is mainly used
# as an input to the autonomy API to then relay this information to the
# autonomy stack.
mosaic_signal(
    name = "vehicle_controller_gps_position_signal",
    proto = "//onboard/signals/vehicle:gps_position_proto",
    proto_message_name = "moz_msg_GPSPosition",
    visibility = ["//visibility:public"],
)
