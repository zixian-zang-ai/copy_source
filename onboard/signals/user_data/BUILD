load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "user_vehicle_settings_topic_proto",
    srcs = ["user_vehicle_settings_topic.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "update_user_vehicle_settings_proto",
    srcs = ["update_user_vehicle_settings.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "update_user_uuid_req_proto",
    srcs = ["update_user_uuid_req.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "user_vehicle_settings_topic_signal",
    proto = "user_vehicle_settings_topic_proto",
    proto_message_name = "moz_msg_UserVehicleSettingsTopic",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "update_user_vehicle_settings_command_signal",
    proto = "update_user_vehicle_settings_proto",
    proto_message_name = "moz_msg_UpdateUserVehicleSettings",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "update_user_uuid_req_signal",
    proto = "update_user_uuid_req_proto",
    proto_message_name = "moz_msg_UpdateUserUuidReq",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "get_user_vehicle_settings_proto",
    srcs = ["get_user_vehicle_settings.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "get_user_vehicle_settings_req_signal",
    proto = ":get_user_vehicle_settings_proto",
    proto_message_name = "moz_msg_GetUserVehicleSettingsReq",
    visibility = ["//visibility:public"],
)
