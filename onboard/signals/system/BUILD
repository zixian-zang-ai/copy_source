load("//onboard/mosaic/signals/rules:defs.bzl", "mosaic_signal", "mosaic_variable_signal")
load("//tools/build:protobuf.bzl", "mosaic_proto_library")

package(default_visibility = ["//visibility:public"])

mosaic_proto_library(
    name = "task_updates_proto",
    srcs = ["task_updates.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_java = True,
    with_nanopb = True,
    with_py = True,
    deps = [":task_info_proto"],
)

mosaic_proto_library(
    name = "task_info_proto",
    srcs = ["task_info.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "touch_event_proto",
    srcs = ["touch_event.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "touch_event_signal",
    proto = "touch_event_proto",
    proto_message_name = "moz_msg_TouchEvent",
)

mosaic_proto_library(
    name = "service_command_proto",
    srcs = ["service_command.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "service_state_proto",
    srcs = ["service_state.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "service_command_signal",
    proto = ":service_command_proto",
    proto_message_name = "moz_msg_ServiceStateChangeCommand",
)

mosaic_signal(
    name = "service_info_response_signal",
    proto = ":service_info_proto",
    proto_message_name = "moz_msg_ServiceInfo",
)

mosaic_signal(
    name = "orchestrator_command_signal",
    proto = ":orchestrator_command_proto",
    proto_message_name = "moz_msg_OrchestratorCommand",
)

mosaic_proto_library(
    name = "orchestrator_command_proto",
    srcs = ["orchestrator_command.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "service_info_proto",
    srcs = ["service_info.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        ":service_state_proto",
        "//onboard/signals/common_types:vehicle_timestamp_proto",
    ],
)

mosaic_proto_library(
    name = "remote_streaming_request_proto",
    srcs = ["remote_streaming_request.proto"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/common_types:camera_proto",
    ],
)

mosaic_signal(
    name = "remote_streaming_request_signal",
    proto = ":remote_streaming_request_proto",
    proto_message_name = "moz_msg_RemoteStreamingRequest",
)

mosaic_proto_library(
    name = "remote_activity_request_proto",
    srcs = ["remote_activity_request.proto"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "remote_activity_request_signal",
    proto = ":remote_activity_request_proto",
    proto_message_name = "moz_msg_RemoteActivityRequest",
    sysml_ids = ["900bc948-a583-438d-abb7-15b7bb0cd6ee"],
)

mosaic_signal(
    name = "task_updates_signal",
    proto = "task_updates_proto",
    proto_message_name = "moz_msg_TaskUpdates",
)

mosaic_proto_library(
    name = "prepare_partitions_request_proto",
    srcs = ["prepare_partitions_request.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "prepare_partitions_request_signal",
    proto = "prepare_partitions_request_proto",
    proto_message_name = "moz_msg_PreparePartitionsRequest",
)

mosaic_proto_library(
    name = "prepare_partitions_response_proto",
    srcs = ["prepare_partitions_response.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "prepare_partitions_response_signal",
    proto = "prepare_partitions_response_proto",
    proto_message_name = "moz_msg_PreparePartitionsResponse",
)

mosaic_proto_library(
    name = "data_logger_session_request_proto",
    srcs = ["data_logger_session_request.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "data_logger_session_request_signal",
    proto = "data_logger_session_request_proto",
    proto_message_name = "moz_msg_DataLoggerSessionRequest",
)

mosaic_proto_library(
    name = "data_logger_session_response_proto",
    srcs = ["data_logger_session_response.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "data_logger_session_response_signal",
    proto = "data_logger_session_response_proto",
    proto_message_name = "moz_msg_DataLoggerSessionResponse",
)

mosaic_proto_library(
    name = "ota_progress_proto",
    srcs = ["ota_progress.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_java = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/hive:vehicle_campaign_status_proto",
    ],
)

mosaic_signal(
    name = "ota_progress_signal",
    proto = "ota_progress_proto",
    proto_message_name = "moz_msg_OtaProgress",
)

mosaic_signal(
    name = "racetrack_logger_request_signal",
    proto = "racetrack_logger_request_proto",
    proto_message_name = "moz_msg_RacetrackLoggerRequest",
)

mosaic_proto_library(
    name = "racetrack_logger_request_proto",
    srcs = ["racetrack_logger_request.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "ota_schedule_install_proto",
    srcs = ["ota_schedule_install.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "ota_schedule_install_signal",
    proto = "ota_schedule_install_proto",
    proto_message_name = "moz_msg_OtaScheduleInstall",
)

mosaic_proto_library(
    name = "ota_progress_request_proto",
    srcs = ["ota_progress_request.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "ota_progress_request_signal",
    proto = "ota_progress_request_proto",
    proto_message_name = "moz_msg_OtaProgressRequest",
)

mosaic_proto_library(
    name = "refresh_data_proto",
    srcs = ["refresh_data.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "refresh_data_signal",
    proto = "refresh_data_proto",
    proto_message_name = "moz_msg_RefreshData",
)

mosaic_signal(
    name = "racetrack_logger_response_signal",
    proto = "racetrack_logger_response_proto",
    proto_message_name = "moz_msg_RacetrackLoggerResponse",
)

mosaic_proto_library(
    name = "restart_partitions_request_proto",
    srcs = ["restart_partitions_request.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "restart_partitions_request_signal",
    proto = "restart_partitions_request_proto",
    proto_message_name = "moz_msg_RestartPartitionsRequest",
)

mosaic_proto_library(
    name = "racetrack_logger_response_proto",
    srcs = ["racetrack_logger_response.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "compute_element_info_proto",
    srcs = [
        "compute_element_info.proto",
    ],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_nanopb = True,
    with_py = True,
    deps = [
        ":service_info_proto",
        "//onboard/signals/common_types:transition_status_proto",
        "//onboard/signals/common_types:vehicle_state_proto",
    ],
)

mosaic_signal(
    name = "compute_element_info_signal",
    proto = "compute_element_info_proto",
    proto_message_name = "moz_msg_ComputeElementState",
)

mosaic_proto_library(
    name = "vehicle_service_heartbeat_proto",
    srcs = ["vehicle_service_heartbeat.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "vehicle_service_heartbeat_signal",
    proto = "vehicle_service_heartbeat_proto",
    proto_message_name = "moz_msg_VehicleServiceHeartbeat",
)

mosaic_proto_library(
    name = "vhal_heartbeat_proto",
    srcs = ["vhal_heartbeat.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "aaos_to_board_signal",
    proto = "vhal_heartbeat_proto",
    proto_message_name = "moz_msg_FromAaosToBoardHeartbeat",
)

mosaic_signal(
    name = "board_to_aaos_signal",
    proto = "vhal_heartbeat_proto",
    proto_message_name = "moz_msg_FromBoardToAaosHeartbeat",
)

mosaic_proto_library(
    name = "hive_connection_proto",
    srcs = ["hive_connection.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "hive_connection_signal",
    proto = "hive_connection_proto",
    proto_message_name = "moz_msg_HiveConnection",
)

mosaic_signal(
    name = "vehicle_service_heartbeat_from_board_signal",
    proto = "vehicle_service_heartbeat_proto",
    proto_message_name = "moz_msg_VehicleServiceHeartbeat",
)

mosaic_proto_library(
    name = "execute_task_proto",
    srcs = ["execute_task.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_java = True,
    with_nanopb = True,
    with_py = True,
    deps = [
        ":task_info_proto",
    ],
)

mosaic_proto_library(
    name = "system_metrics_recording_proto",
    srcs = ["system_metrics_recording.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_nanopb = True,
    with_py = True,
    deps = [
        ":task_info_proto",
    ],
)

mosaic_variable_signal(
    name = "execute_task_signal",
    proto = "execute_task_proto",
    proto_message_name = "moz_msg_ExecuteTask",
    variants = [
        "android",
        "central",
        "adas",
        "adas_2",
        "front",
        "rear",
        "stack_pc",
    ],
)

mosaic_signal(
    name = "system_metrics_recording_request_signal",
    proto = "system_metrics_recording_proto",
    proto_message_name = "moz_msg_SystemMetricsRecordingRequest",
)

mosaic_signal(
    name = "system_metrics_recording_response_signal",
    proto = "system_metrics_recording_proto",
    proto_message_name = "moz_msg_SystemMetricsRecordingResponse",
)

mosaic_proto_library(
    name = "system_usage_proto",
    srcs = ["system_usage.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "cpu_usage_signal",
    proto = "system_usage_proto",
    proto_message_name = "moz_msg_CpuUsage",
)

mosaic_signal(
    name = "disk_usage_signal",
    proto = "system_usage_proto",
    proto_message_name = "moz_msg_DiskUsage",
)

mosaic_signal(
    name = "memory_usage_signal",
    proto = "system_usage_proto",
    proto_message_name = "moz_msg_MemoryUsage",
)

mosaic_signal(
    name = "apk_memory_usage_signal",
    proto = "system_usage_proto",
    proto_message_name = "moz_msg_ApkMemoryUsage",
)

mosaic_signal(
    name = "apk_cpu_usage_signal",
    proto = "system_usage_proto",
    proto_message_name = "moz_msg_ApkCpuUsage",
)

mosaic_proto_library(
    name = "android_capabilities_proto",
    srcs = ["android_capabilities.proto"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "android_capabilities_signal",
    proto = "android_capabilities_proto",
    proto_message_name = "moz_msg_AndroidCapabilities",
)

mosaic_proto_library(
    name = "dashcam_recording_proto",
    srcs = ["dashcam_recording.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "dashcam_record_command_signal",
    proto = "dashcam_recording_proto",
    proto_message_name = "moz_msg_DashcamRecordCommand",
)

mosaic_signal(
    name = "dashcam_recording_state_signal",
    proto = "dashcam_recording_proto",
    proto_message_name = "moz_msg_DashcamRecordingState",
)

mosaic_signal(
    name = "delete_dashcam_recording_command_signal",
    proto = "dashcam_recording_proto",
    proto_message_name = "moz_msg_DeleteDashcamRecordingCommand",
)

mosaic_proto_library(
    name = "logging_rule_update_proto",
    srcs = ["logging_rule_update.proto"],
    proto_option_deps = [
        "@com_github_nanopb_nanopb//:nanopb_proto",
    ],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "logging_rule_update_signal",
    proto = "logging_rule_update_proto",
    proto_message_name = "moz_msg_LoggingRuleUpdate",
)

mosaic_proto_library(
    name = "board_target_versions_request_proto",
    srcs = ["board_target_versions_request.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "board_target_versions_request_signal",
    proto = "board_target_versions_request_proto",
    proto_message_name = "moz_msg_BoardTargetVersionsRequest",
)

mosaic_proto_library(
    name = "board_target_versions_response_proto",
    srcs = ["board_target_versions_response.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "board_target_versions_response_signal",
    proto = "board_target_versions_response_proto",
    proto_message_name = "moz_msg_BoardTargetVersionsResponse",
)

mosaic_proto_library(
    name = "android_gnss_heartbeat_proto",
    srcs = ["android_gnss_heartbeat.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    with_cc = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "gnss_to_board_signal",
    proto = "android_gnss_heartbeat_proto",
    proto_message_name = "moz_msg_FromGnssToBoardHeartbeat",
)

mosaic_signal(
    name = "board_to_gnss_signal",
    proto = "android_gnss_heartbeat_proto",
    proto_message_name = "moz_msg_FromBoardToGnssHeartbeat",
)

mosaic_proto_library(
    name = "text_to_intent_request_proto",
    srcs = ["text_to_intent_request.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    with_nanopb = True,
    with_py = True,
)

mosaic_signal(
    name = "text_to_intent_request_signal",
    proto = "text_to_intent_request_proto",
    proto_message_name = "moz_msg_TextToIntentRequest",
)

mosaic_proto_library(
    name = "text_to_intent_response_proto",
    srcs = ["text_to_intent_response.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    with_nanopb = True,
    with_py = True,
    deps = [
        "//onboard/signals/hive:intent",
    ],
)

mosaic_signal(
    name = "text_to_intent_response_signal",
    proto = "text_to_intent_response_proto",
    proto_message_name = "moz_msg_TextToIntentResponse",
)

mosaic_proto_library(
    name = "system_manifest_proto",
    srcs = ["system_manifest.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    with_cc = True,
    with_java = True,
    with_nanopb = True,
    with_py = True,
)

mosaic_proto_library(
    name = "install_manager_service_proto",
    srcs = ["install_manager_service.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    with_cc = True,
    with_nanopb = True,
    deps = [
        ":system_manifest_proto",
    ],
)

mosaic_proto_library(
    name = "install_worker_service_proto",
    srcs = ["install_worker_service.proto"],
    proto_option_deps = ["@com_github_nanopb_nanopb//:nanopb_proto"],
    with_cc = True,
    with_nanopb = True,
    deps = [
        ":system_manifest_proto",
    ],
)

mosaic_signal(
    name = "install_manager_state_info_signal",
    proto = "install_manager_service_proto",
    proto_message_name = "moz_msg_InstallManagerStateInfo",
)

mosaic_signal(
    name = "create_manifest_signal",
    proto = "install_manager_service_proto",
    proto_message_name = "moz_msg_CreateManifest",
)

mosaic_signal(
    name = "complete_manifest_signal",
    proto = "install_manager_service_proto",
    proto_message_name = "moz_msg_CompleteManifest",
)

mosaic_signal(
    name = "apply_manifest_signal",
    proto = "install_manager_service_proto",
    proto_message_name = "moz_msg_ApplyManifest",
)

mosaic_signal(
    name = "reap_manifest_signal",
    proto = "install_manager_service_proto",
    proto_message_name = "moz_msg_ReapManifest",
)

mosaic_signal(
    name = "install_worker_state_info_signal",
    proto = "install_worker_service_proto",
    proto_message_name = "moz_msg_InstallWorkerStateInfo",
)

mosaic_variable_signal(
    name = "rollback_install_signal",
    proto = "install_manager_service_proto",
    proto_message_name = "moz_msg_RollbackInstall",
    variants = [
        "android",
        "central",
        "adas",
        "adas_2",
        "front",
        "rear",
        "stack_pc",
    ],
)

mosaic_variable_signal(
    name = "deploy_install_signal",
    proto = "install_manager_service_proto",
    proto_message_name = "moz_msg_DeployInstall",
    variants = [
        "android",
        "central",
        "adas",
        "adas_2",
        "front",
        "rear",
        "stack_pc",
    ],
)

mosaic_variable_signal(
    name = "reap_deploy_signal",
    proto = "install_manager_service_proto",
    proto_message_name = "moz_msg_ReapDeploy",
    variants = [
        "android",
        "central",
        "adas",
        "adas_2",
        "front",
        "rear",
        "stack_pc",
    ],
)

mosaic_variable_signal(
    name = "reap_install_signal",
    proto = "install_manager_service_proto",
    proto_message_name = "moz_msg_ReapInstall",
    variants = [
        "android",
        "central",
        "adas",
        "adas_2",
        "front",
        "rear",
        "stack_pc",
    ],
)

mosaic_variable_signal(
    name = "commit_install_signal",
    proto = "install_manager_service_proto",
    proto_message_name = "moz_msg_CommitInstall",
    variants = [
        "android",
        "central",
        "adas",
        "adas_2",
        "front",
        "rear",
        "stack_pc",
    ],
)
