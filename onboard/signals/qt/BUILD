load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

#-------- PROTOS start --------
mosaic_proto_library(
    name = "qt_app_state_proto",
    srcs = ["qt_app_state.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "qt_lifecycle_command_proto",
    srcs = ["qt_lifecycle_command.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "qt_lifecycle_status_proto",
    srcs = ["qt_lifecycle_status.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "qt_camera_proto",
    srcs = [
        "qt_camera.proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "qt_boot_animation_status_proto",
    srcs = [
        "qt_boot_animation_status.proto",
    ],
    visibility = ["//visibility:public"],
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

#-------- PROTOS end --------

#-------- SIGNALS start --------
mosaic_signal(
    name = "sentry_qt_app_transition_signal",
    proto = "qt_lifecycle_command_proto",
    proto_message_name = "moz_msg_QtLifecycleCommand",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "sentry_qt_lifecycle_command_signal",
    proto = "qt_lifecycle_command_proto",
    proto_message_name = "moz_msg_QtLifecycleCommand",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "off_screen_qt_lifecycle_command_signal",
    proto = "qt_lifecycle_command_proto",
    proto_message_name = "moz_msg_QtLifecycleCommand",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "off_screen_qt_lifecycle_status_signal",
    proto = "qt_lifecycle_status_proto",
    proto_message_name = "moz_msg_QtLifecycleStatus",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "boot_screen_qt_lifecycle_command_signal",
    proto = "qt_lifecycle_command_proto",
    proto_message_name = "moz_msg_QtLifecycleCommand",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "boot_screen_qt_lifecycle_status_signal",
    proto = "qt_lifecycle_status_proto",
    proto_message_name = "moz_msg_QtLifecycleStatus",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "cluster_qt_lifecycle_command_signal",
    proto = "qt_lifecycle_command_proto",
    proto_message_name = "moz_msg_QtLifecycleCommand",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "cluster_qt_lifecycle_status_signal",
    proto = "qt_lifecycle_status_proto",
    proto_message_name = "moz_msg_QtLifecycleStatus",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "camera_viewer_command_signal",
    proto = "qt_camera_proto",
    proto_message_name = "moz_msg_QtCameraViewerCommand",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "camera_status_signal",
    proto = "qt_camera_proto",
    proto_message_name = "moz_msg_QtCameraStatus",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "boot_animation_signal",
    proto = "qt_boot_animation_status_proto",
    proto_message_name = "moz_msg_QtBootAnimationStatus",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "install_progress_screen_qt_lifecycle_status_signal",
    proto = "qt_lifecycle_status_proto",
    proto_message_name = "moz_msg_QtLifecycleStatus",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "install_progress_screen_qt_lifecycle_command_signal",
    proto = "qt_lifecycle_command_proto",
    proto_message_name = "moz_msg_QtLifecycleCommand",
    visibility = ["//visibility:public"],
)

#-------- SIGNALS END --------
