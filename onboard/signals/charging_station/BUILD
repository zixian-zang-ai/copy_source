load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "mmcr_proto",
    srcs = ["mmcr.proto"],
    visibility = ["//visibility:public"],
    with_java = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:si_units_proto",
    ],
)

mosaic_signal(
    name = "mmcr_charging_station_signal",
    proto = "mmcr_proto",
    proto_message_name = "moz_msg_ChargingStation",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "mmcr_charge_ready_activation_signal",
    proto = "mmcr_proto",
    proto_message_name = "moz_msg_ChargeReadyActivation",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "battery_thermal_management_state_signal",
    proto = "mmcr_proto",
    proto_message_name = "moz_msg_BatteryThermalManagementState",
    visibility = ["//visibility:public"],
)

mosaic_signal(
    name = "battery_thermal_management_request_signal",
    proto = "mmcr_proto",
    proto_message_name = "moz_msg_BatteryThermalManagementRequest",
    visibility = ["//visibility:public"],
)
