load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

# camera_heartbeat_proto
mosaic_proto_library(
    name = "camera_heartbeat_proto",
    srcs = ["camera_heartbeat.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:vehicle_timestamp_proto",
    ],
)

mosaic_signal(
    name = "right_side_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "left_side_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "rear_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "front_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "cabin_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "front_left_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "front_right_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "adas_front_left_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "adas_front_right_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "adas_rear_left_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "adas_rear_right_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "adas_front_center_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "adas_rear_center_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "adas_front_center_cabin_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "surround_view_camera_heartbeat_signal",
    proto = "camera_heartbeat_proto",
    proto_message_name = "moz_msg_CameraHeartbeat",
    visibility = ["//visibility:public"],
)

# switch_buffer_request_proto
mosaic_proto_library(
    name = "switch_buffer_request_proto",
    srcs = ["switch_buffer_request.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "front_switch_buffer_request_signal",
    proto = "switch_buffer_request_proto",
    proto_message_name = "moz_msg_SwitchBufferRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "rear_switch_buffer_request_signal",
    proto = "switch_buffer_request_proto",
    proto_message_name = "moz_msg_SwitchBufferRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "right_side_switch_buffer_request_signal",
    proto = "switch_buffer_request_proto",
    proto_message_name = "moz_msg_SwitchBufferRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "left_side_switch_buffer_request_signal",
    proto = "switch_buffer_request_proto",
    proto_message_name = "moz_msg_SwitchBufferRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "cabin_switch_buffer_request_signal",
    proto = "switch_buffer_request_proto",
    proto_message_name = "moz_msg_SwitchBufferRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "surround_view_switch_buffer_request_signal",
    proto = "switch_buffer_request_proto",
    proto_message_name = "moz_msg_SwitchBufferRequest",
    visibility = ["//visibility:public"],
)

# camera_frame_proto
mosaic_proto_library(
    name = "camera_format_proto",
    srcs = ["camera_format.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        ":camera_timestamp_proto",
    ],
)

mosaic_signal(
    name = "front_camera_format_signal",
    proto = "camera_format_proto",
    proto_message_name = "moz_msg_CameraFormat",
    sysml_ids = [],
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "rear_camera_format_signal",
    proto = "camera_format_proto",
    proto_message_name = "moz_msg_CameraFormat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "cabin_camera_format_signal",
    proto = "camera_format_proto",
    proto_message_name = "moz_msg_CameraFormat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "right_side_camera_format_signal",
    proto = "camera_format_proto",
    proto_message_name = "moz_msg_CameraFormat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "left_side_camera_format_signal",
    proto = "camera_format_proto",
    proto_message_name = "moz_msg_CameraFormat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "front_left_camera_format_signal",
    proto = "camera_format_proto",
    proto_message_name = "moz_msg_CameraFormat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "front_right_camera_format_signal",
    proto = "camera_format_proto",
    proto_message_name = "moz_msg_CameraFormat",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "surround_view_camera_format_signal",
    proto = "camera_format_proto",
    proto_message_name = "moz_msg_CameraFormat",
    visibility = ["//visibility:public"],
)

# image protos
mosaic_proto_library(
    name = "image_proto",
    srcs = ["image.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        ":camera_format_proto",
        ":camera_timestamp_proto",
    ],
)

mosaic_proto_library(
    name = "camera_timestamp_proto",
    srcs = ["camera_timestamp.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:vehicle_timestamp_proto",
    ],
)

cameras = [
    "front",
    "rear",
    "right_side",
    "left_side",
    "cabin",
    "adas_front_left",
    "adas_front_right",
    "adas_rear_left",
    "adas_rear_right",
    "adas_front_center",
    "adas_rear_center",
    "adas_front_center_cabin",
    "front_left",
    "front_right",
    "surround_view",
]

# TODO(Eesha): Redo these for new camera implementation
stream_sysml_ids = {
    "front": [
        "285293bf-2f42-4f8a-91a7-b33870df9216",
    ],
    "rear": [
        "af5eec09-70ec-4928-b49f-2386bf7aac02",
    ],
    "right_side": [
        "be0a351f-fcb1-4f83-897f-1dbb17f34f47",
    ],
    "left_side": ["e96a3476-87e9-4637-8d7e-dfe713ab8fcb"],
    "cabin": [
        "f8da3b0e-2549-4138-a7ed-d239946c5bfc",
    ],
}

[
    mosaic_signal(
        name = "{}_camera_frame_signal".format(camera),
        proto = "//onboard/signals/common_types:chunked_message_proto",
        proto_message_name = "moz_msg_ChunkedMessage",
        sysml_ids = stream_sysml_ids[camera] if camera in stream_sysml_ids else [],
        visibility = ["//visibility:public"],
    )
    for camera in cameras
]

mosaic_signal(
    name = "zedfas_stitched_frame_signal",
    proto = "//onboard/signals/common_types:chunked_message_proto",
    proto_message_name = "moz_msg_ChunkedMessage",
    visibility = ["//visibility:public"],
)

# Camera Manager Active Cameras
mosaic_proto_library(
    name = "onboard_cameras_proto",
    srcs = ["onboard_cameras.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "onboard_cameras_signal",
    proto = "onboard_cameras_proto",
    proto_message_name = "moz_msg_OnboardCameras",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "onboard_cameras_request_proto",
    srcs = ["onboard_cameras_request.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "onboard_cameras_request_signal",
    proto = "onboard_cameras_request_proto",
    proto_message_name = "moz_msg_OnboardCamerasRequest",
    visibility = ["//visibility:public"],
)
