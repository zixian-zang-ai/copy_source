load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

mosaic_proto_library(
    name = "toggle_valet_mode_request_proto",
    srcs = ["toggle_valet_mode_request.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "toggle_valet_mode_request_signal",
    proto = "toggle_valet_mode_request_proto",
    proto_message_name = "moz_msg_ToggleValetModeRequest",
    sysml_ids = ["e682d85a-0a12-4049-a96a-91822569d21d"],
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "toggle_valet_mode_response_proto",
    srcs = ["toggle_valet_mode_response.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_java = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        ":valet_mode_state_proto",
    ],
)

mosaic_signal(
    name = "toggle_valet_mode_response_signal",
    proto = "toggle_valet_mode_response_proto",
    proto_message_name = "moz_msg_ToggleValetModeResponse",
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "valet_mode_state_proto",
    srcs = ["valet_mode_state.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "valet_mode_state_signal",
    proto = "valet_mode_state_proto",
    proto_message_name = "moz_msg_ValetModeState",
    sysml_ids = ["b4c82e81-8567-4682-afea-cafad2c57b12"],
    visibility = ["//visibility:public"],
)

mosaic_proto_library(
    name = "get_valet_mode_state_request_proto",
    srcs = ["get_valet_mode_state_request.proto"],
    visibility = ["//visibility:public"],
    with_cc = True,
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "get_valet_mode_state_request_signal",
    proto = "get_valet_mode_state_request_proto",
    proto_message_name = "moz_msg_GetValetModeStateRequest",
    visibility = ["//visibility:public"],
)
