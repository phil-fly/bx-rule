# bx-rule
百晓HIDS规则


# ATT&CK覆盖

## discovery
### t1087.001
- [Local System Accounts Discovery](rules/linux/process/lnx_local_account.jsonlnx_local_account.json)
### t1069.001
- [Local Groups Discovery](rules/linux/process/lnx_local_groups.json)

### t1046
- [Linux Network Service Scanning](rules/linux/process/lnx_network_service_scanning.yml)

### t1057
- [Process Discovery](rules/linux/process/lnx_process_discovery.yml)

### t1018
- [Linux Remote System Discovery](rules/linux/process/lnx_remote_system_discovery.json)

### t1518.001
- [Security Software Discovery](rules/linux/process/lnx_security_software_discovery.yml)

### t1082
- [System Information Discovery](rules/linux/process/lnx_system_info_discovery.yml)

### t1049
- [system network connections discovery](rules/linux/process/lnx_system_network_connections_discovery.yml)

### t1016
- [System Network Discovery](rules/linux/process/lnx_system_network_discovery.yml)

### t1083
- [File and Directory Discovery](rules/linux/process/lnx_file_and_directory_discovery.yml)

## lateral_movement

### t1105 (Ingress Tool Transfer)
- [Remote File Copy](rules/linux/process/lnx_file_copy.yml)

## defense_evasion
### t1027 (Obfuscated Files or InformationObfuscated Files or Information)
- [Decode Base64 Encoded Text](rules/linux/process/lnx_base64_decode.yml)

### t1070.004
- [File Deletion](rules/linux/process/lnx_file_deletion.yml)

### xxx
- [Connection Proxy](rules/linux/process/lnx_proxy_connection.yml)

### t1562.004
- [Disabling Security Tools](rules/linux/process/lnx_security_tools_disabling.yml)

### t1222.001
- [File and Directory Permissions Modification](rules/linux/file/lnx_file_and_dir_perm_mod.yml)


## privilege_escalation
### t1548.001
- [Setuid and Setgid](rules/linux/process/lnx_setgid_setuid.yml)
- [Suid Privilege Escalation](rules/linux/process/lnx_suid.yml)

### t1611 (Escape to Host 虚机逃逸)
- [container逃逸](rules/linux/process/container_escape_for_Docker.yml)
- [通过错误配置使用定时任务逃逸](rules/linux/process/container_escape_for_Docker1.yml)

## execution

### 1053.003
- [Scheduled Cron Task/Job](rules/linux/process/lnx_schedule_task_job_cron.yml)


## persistence
### 1053.003
- [Scheduled Cron Task/Job](rules/linux/process/lnx_schedule_task_job_cron.yml)

### t1136.001
- [Creation Of A Local User Account](rules/linux/process/lnx_create_account.yml)
