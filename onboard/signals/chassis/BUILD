load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "brake_request_proto",
    srcs = ["brake_request.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "brake_request_signal",
    proto = "brake_request_proto",
    proto_message_name = "moz_msg_BrakeRequest",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "trunk_state_proto",
    srcs = ["trunk_state.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "trunk_state_signal",
    proto = "trunk_state_proto",
    proto_message_name = "moz_msg_TrunkState",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "trunk_measured_state_signal",
    proto = "trunk_state_proto",
    proto_message_name = "moz_msg_TrunkState",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "gear_intent_proto",
    srcs = ["gear_intent.proto"],
    visibility = ["//visibility:public"],
    with_go = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "gear_intent_signal",
    proto = "gear_intent_proto",
    proto_message_name = "moz_msg_GearIntent",
    sysml_ids = ["9da06f9b-0a42-4fa6-9a39-84e4beecfd09"],
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "gear_state_proto",
    srcs = ["gear_state.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "gear_intent_response_signal",
    proto = "gear_intent_proto",
    proto_message_name = "moz_msg_GearIntentResponse",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "gear_state_signal",
    proto = "gear_state_proto",
    proto_message_name = "moz_msg_GearState",
    sysml_ids = ["df0be0f8-0e53-45bd-a31c-059b993a77a1"],
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "vehicle_acceleration_proto",
    srcs = ["vehicle_acceleration.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "vehicle_acceleration_signal",
    proto = "vehicle_acceleration_proto",
    proto_message_name = "moz_msg_VehicleAcceleration",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "rear_steering_command_proto",
    srcs = ["rear_steering_command.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "rear_steering_command_signal",
    proto = "rear_steering_command_proto",
    proto_message_name = "moz_msg_RearSteeringCommand",
    sysml_ids = ["66f83b87-1894-49df-a340-615e272f9588"],
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "steering_test_mode_proto",
    srcs = ["steering_test_mode.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "steering_test_mode_signal",
    proto = "steering_test_mode_proto",
    proto_message_name = "moz_msg_SteeringTestMode",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "steering_fault_status_proto",
    srcs = ["steering_fault_status.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "steering_fault_status_signal",
    proto = "steering_fault_status_proto",
    proto_message_name = "moz_msg_SteeringFaultStatus",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "brake_system_command_proto",
    srcs = ["brake_system_command.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_signal(
    name = "brake_system_command_signal",
    proto = "brake_system_command_proto",
    proto_message_name = "moz_msg_BrakeSystemCommand",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "steering_by_wire_proto",
    srcs = ["steering_by_wire.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_signal(
    name = "steering_by_wire_signal",
    proto = "steering_by_wire_proto",
    proto_message_name = "moz_msg_SteeringByWire",
    visibility = ["//visibility:public"],
)

##############
###  Tires ###
##############

mosaic_proto_library(
    name = "tire_pressure_proto",
    srcs = ["tire_pressure.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_signal(
    name = "front_left_tire_pressure_signal",
    proto = "tire_pressure_proto",
    proto_message_name = "moz_msg_TirePressure",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "front_right_tire_pressure_signal",
    proto = "tire_pressure_proto",
    proto_message_name = "moz_msg_TirePressure",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "rear_left_tire_pressure_signal",
    proto = "tire_pressure_proto",
    proto_message_name = "moz_msg_TirePressure",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "rear_right_tire_pressure_signal",
    proto = "tire_pressure_proto",
    proto_message_name = "moz_msg_TirePressure",
    visibility = ["//visibility:public"],
)
