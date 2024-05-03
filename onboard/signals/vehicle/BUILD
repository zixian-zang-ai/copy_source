load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_signal(
    name = "vehicle_speed_signal",
    proto = "vehicle_speed_proto",
    proto_message_name = "moz_msg_VehicleSpeed",
    sysml_ids = ["b2c756c1-5581-44da-907d-ca3a5b3ffb5e"],
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "vehicle_speed_proto",
    srcs = ["vehicle_speed.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_proto_library(
    name = "vehicle_acceleration_command_proto",
    srcs = ["vehicle_acceleration_command.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "vehicle_acceleration_command_signal",
    proto = "vehicle_acceleration_command_proto",
    proto_message_name = "moz_msg_VehicleAccelerationCommand",
    sysml_ids = ["99906005-b2ea-459e-b1b3-ddad537a66d0"],
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "vehicle_range_proto",
    srcs = ["vehicle_range.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_proto_library(
    name = "brake_torque_proto",
    srcs = ["brake_torque.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "brake_intent_proto",
    srcs = ["brake_intent.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "brake_intent_signal",
    proto = "brake_intent_proto",
    proto_message_name = "moz_msg_BrakeIntent",
    sysml_ids = ["517a0f24-e15d-409d-b92b-b8d6f4b732d9"],
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "vehicle_range_signal",
    proto = "vehicle_range_proto",
    proto_message_name = "moz_msg_VehicleRange",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "odometer_distance_proto",
    srcs = ["odometer_distance.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_signal(
    name = "odometer_distance_signal",
    proto = "odometer_distance_proto",
    proto_message_name = "moz_msg_OdometerDistance",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "brake_torque_signal",
    proto = "brake_torque_proto",
    proto_message_name = "moz_msg_BrakeTorque",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "charge_info_proto",
    srcs = ["charge_info.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_proto_library(
    name = "charging_command_proto",
    srcs = ["charging_command.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "power_state_proto",
    srcs = ["power_state.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "vehicle_power_state_signal",
    proto = "power_state_proto",
    proto_message_name = "moz_msg_VehiclePowerState",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "charge_info_signal",
    proto = "charge_info_proto",
    proto_message_name = "moz_msg_ChargeInfo",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "charging_command_signal",
    proto = "charging_command_proto",
    proto_message_name = "moz_msg_ChargingCommand",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "charging_status_signal",
    proto = "charge_info_proto",
    proto_message_name = "moz_msg_ChargingStatus",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "gps_position_proto",
    srcs = ["gps_position.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "gps_position_signal",
    proto = "gps_position_proto",
    proto_message_name = "moz_msg_GPSPosition",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "energy_recuperation_proto",
    srcs = ["energy_recuperation.proto"],
    visibility = ["//visibility:public"],
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "set_recuperation_request_signal",
    proto = "energy_recuperation_proto",
    proto_message_name = "moz_msg_SetRecuperationRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "recuperation_intensity_state_signal",
    proto = "energy_recuperation_proto",
    proto_message_name = "moz_msg_RecuperationIntensityState",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "vehicle_settings_ui_proto",
    srcs = ["vehicle_settings_ui.proto"],
    visibility = ["//visibility:public"],
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "set_steer_feel_mode_request_signal",
    proto = "vehicle_settings_ui_proto",
    proto_message_name = "moz_msg_SetSteerFeelModeRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "steer_feel_mode_state_signal",
    proto = "vehicle_settings_ui_proto",
    proto_message_name = "moz_msg_SteerFeelModeState",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "set_acc_pedal_mode_request_signal",
    proto = "vehicle_settings_ui_proto",
    proto_message_name = "moz_msg_SetAccPedalModeRequest",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "acc_pedal_mode_state_signal",
    proto = "vehicle_settings_ui_proto",
    proto_message_name = "moz_msg_AccPedalModeState",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "accel_gyro_signal",
    proto = "accel_gyro_proto",
    proto_message_name = "moz_msg_AccelGyro",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "accel_gyro_proto",
    srcs = ["accel_gyro.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "vehicle_rotation_signal",
    proto = "vehicle_rotation_proto",
    proto_message_name = "moz_msg_VehicleRotation",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "vehicle_rotation_proto",
    srcs = ["vehicle_rotation.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "pedal_position_proto",
    srcs = ["pedal_position.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "pedal_position_signal",
    proto = "pedal_position_proto",
    proto_message_name = "moz_msg_PedalPosition",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "steering_angle_proto",
    srcs = ["steering_angle.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "steering_angle_signal",
    proto = "steering_angle_proto",
    proto_message_name = "moz_msg_SteeringAngle",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "wheel_info_proto",
    srcs = ["wheel_info.proto"],
    visibility = ["//visibility:public"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_signal(
    name = "wheel_info_signal",
    proto = "wheel_info_proto",
    proto_message_name = "moz_msg_WheelInfo",
    visibility = ["//visibility:public"],
)
