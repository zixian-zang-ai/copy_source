load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "traffic_light_state_proto",
    srcs = ["traffic_light_state.proto"],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "traffic_light_state_signal",
    proto = "traffic_light_state_proto",
    proto_message_name = "moz_msg_TrafficLightState",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "adas_driving_command_proto",
    srcs = ["adas_driving_command.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_signal(
    name = "adas_steering_command_signal",
    proto = "adas_driving_command_proto",
    proto_message_name = "moz_msg_AdasSteeringCommand",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "adas_intent_proto",
    srcs = ["adas_intent.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "adas_intent_signal",
    proto = "adas_intent_proto",
    proto_message_name = "moz_msg_AdasIntent",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "adas_state_proto",
    srcs = ["adas_state.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "adas_state_signal",
    proto = "adas_state_proto",
    proto_message_name = "moz_msg_AdasState",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "image_and_detections_proto",
    srcs = ["image_and_detections.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/camera:camera_format_proto",
        "//onboard/signals/camera:image_proto",
    ],
)

mosaic_signal(
    name = "adas_image_and_detection_signal",
    proto = "image_and_detections_proto",
    proto_message_name = "moz_msg_ImageAndDetections",
    visibility = ["//visibility:public"],
)

# adas brake request
mosaic_proto_library(
    name = "adas_brake_request_proto",
    srcs = ["adas_brake_request.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "adas_brake_request_signal",
    proto = "adas_brake_request_proto",
    proto_message_name = "moz_msg_AdasBrakeRequest",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "adaptive_cruise_control_hmi_status_proto",
    srcs = ["adaptive_cruise_control_hmi_status.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_signal(
    name = "adaptive_cruise_control_hmi_status_signal",
    proto = "adaptive_cruise_control_hmi_status_proto",
    proto_message_name = "moz_msg_AdaptiveCruiseControlHmiStatus",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "lane_keep_assist_hmi_status_proto",
    srcs = ["lane_keep_assist_hmi_status.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/body:blinker_state_proto",
    ],
)

mosaic_signal(
    name = "lane_keep_assist_hmi_status_signal",
    proto = "lane_keep_assist_hmi_status_proto",
    proto_message_name = "moz_msg_LaneKeepAssistHmiStatus",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "front_camera_detections_signal".format(camera),
    proto = "image_and_detections_proto",
    proto_message_name = "moz_msg_ImageDetections",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "left_side_camera_detections_signal".format(camera),
    proto = "image_and_detections_proto",
    proto_message_name = "moz_msg_ImageDetections",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "right_side_side_camera_detections_signal".format(camera),
    proto = "image_and_detections_proto",
    proto_message_name = "moz_msg_ImageDetections",
    visibility = ["//visibility:public"],
)
