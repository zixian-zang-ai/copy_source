load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "beam_stalk_state_proto",
    srcs = ["beam_stalk_state.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "user_ble_proximity_proto",
    srcs = ["user_ble_proximity.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "light_color_update_proto",
    srcs = ["light_color_update.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "cabin_light_color_update_signal",
    proto = "light_color_update_proto",
    proto_message_name = "moz_msg_LightColorUpdate",
    sysml_ids = ["08df4ebf-9163-4c87-91c0-d80f1519f8a1"],
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "steering_button_state_proto",
    srcs = ["steering_button_state.proto"],
    visibility = ["//visibility:public"],
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "beam_stalk_state_signal",
    proto = "beam_stalk_state_proto",
    proto_message_name = "moz_msg_BeamStalkState",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "user_ble_proximity_signal",
    proto = "user_ble_proximity_proto",
    proto_message_name = "moz_msg_UserBleProximity",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "sentry_command_proto",
    srcs = ["sentry_command.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "sentry_command_signal",
    proto = "sentry_command_proto",
    proto_message_name = "moz_msg_SentryCommand",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "sentry_command_ack_signal",
    proto = "sentry_command_proto",
    proto_message_name = "moz_msg_SentryCommandAck",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "steering_hid_inputs_proto",
    srcs = ["steering_hid_inputs.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    visibility = ["//visibility:public"],
    with_java = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        ":steering_button_state_proto",
    ],
)

mosaic_signal(
    name = "steering_hid_inputs_signal",
    proto = "steering_hid_inputs_proto",
    proto_message_name = "moz_msg_SteeringHIDInputs",
    visibility = ["//visibility:public"],
)

#######################
###  Cabin Lighting ###
#######################

mosaic_signal(
    name = "surround_rgb_strip_state_signal",
    proto = "//onboard/signals/common_types:light_schedule_proto",
    proto_message_name = "moz_msg_LightState",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "dash_rgb_strip_state_signal",
    proto = "//onboard/signals/common_types:light_schedule_proto",
    proto_message_name = "moz_msg_LightState",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "surround_rgb_strip_command_signal",
    proto = "//onboard/signals/common_types:light_schedule_proto",
    proto_message_name = "moz_msg_LightSchedule",
    sysml_ids = ["08df4ebf-9163-4c87-91c0-d80f1519f8a1"],
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "dash_rgb_strip_command_signal",
    proto = "//onboard/signals/common_types:light_schedule_proto",
    proto_message_name = "moz_msg_LightSchedule",
    sysml_ids = ["08df4ebf-9163-4c87-91c0-d80f1519f8a1"],
    visibility = ["//visibility:public"],
)

#######################
###       HVAC      ###
#######################

mosaic_proto_library(
    name = "hvac_proto",
    srcs = ["hvac.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_signal(
    name = "hvac_temperature_info_signal",
    proto = "hvac_proto",
    proto_message_name = "moz_msg_HvacTemperatureInfo",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "hvac_fan_status_signal",
    proto = "hvac_proto",
    proto_message_name = "moz_msg_HvacFanStatus",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "hvac_air_circulation_button_state_signal",
    proto = "hvac_proto",
    proto_message_name = "moz_msg_HvacAirCirculationButtonState",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "hvac_seat_setting_signal",
    proto = "hvac_proto",
    proto_message_name = "moz_msg_HvacSeatSetting",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "hvac_info_from_app_signal",
    proto = "hvac_proto",
    proto_message_name = "moz_msg_HvacAppInfo",
    sysml_ids = [
        "4d5dc384-c8b6-493f-8262-1bc3f510fce6",
        "2a81d103-9c10-4b60-851a-8fba8b379cba",
    ],
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "hvac_info_to_app_signal",
    proto = "hvac_proto",
    proto_message_name = "moz_msg_HvacAppInfo",
    sysml_ids = ["dd8e02a2-6172-49fa-b79d-143ac49dd2d3"],
    visibility = ["//visibility:public"],
)

#######################################
###       PRECONDITION MANAGER      ###
#######################################

mosaic_proto_library(
    name = "precondition_manager_proto",
    srcs = ["precondition_manager.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_java = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_signal(
    name = "add_request_signal",
    proto = "precondition_manager_proto",
    proto_message_name = "moz_msg_PreconditionManagerAddRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "cancel_current_request_signal",
    proto = "precondition_manager_proto",
    proto_message_name = "moz_msg_PreconditionManagerCancelCurrentRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "cancel_scheduled_request_signal",
    proto = "precondition_manager_proto",
    proto_message_name = "moz_msg_PreconditionManagerCancelScheduledRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "publish_precondition_state_signal",
    proto = "precondition_manager_proto",
    proto_message_name = "moz_msg_PreconditionManagerPublishState",
    visibility = ["//visibility:public"],
)
