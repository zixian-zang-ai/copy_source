load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_signal(
    name = "power_button_state_signal",
    proto = "//onboard/signals/common_types:button_state_proto",
    proto_message_name = "moz_msg_ButtonState",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "propulsion_power_signal",
    proto = "//onboard/signals/powertrain:propulsion_power_proto",
    proto_message_name = "moz_msg_PropulsionPower",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "propulsion_power_proto",
    srcs = ["propulsion_power.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "torque_path_command_proto",
    srcs = ["torque_path_command.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_signal(
    name = "torque_path_command_signal",
    proto = "torque_path_command_proto",
    proto_message_name = "moz_msg_TorquePathCommand",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "electric_motor_torque_proto",
    srcs = ["electric_motor_torque.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_signal(
    name = "electric_motor_torque_signal",
    proto = "electric_motor_torque_proto",
    proto_message_name = "moz_msg_ElectricMotorTorque",
    visibility = ["//visibility:public"],
)
