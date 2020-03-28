# Config Validator Constraint Templates

Constraint templates specify the logic to be used by constraints.
This repository contains pre-defined constraint templates that you can implement or modify for your own needs. 

## Creating a constraint template
You can create and implement your own custom constraint templates.
For instructions on how to write constraint templates, see [How to write your own constraint templates](./constraint_template_authoring.md).

## Available Templates

| Template                                                                                                                                        | Samples                                                                                                                          |
| ----------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| [GCPAlwaysViolatesConstraintV1](../../policies/templates/gcp_always_violates_v1.yaml)                                                           |                                                                                                                                  |
| [GCPAppengineLocationConstraintV1](../../policies/templates/gcp_appengine_location_v1.yaml)                                                     |                                                                                                                                  |
| [GCPBigQueryDatasetLocationConstraintV1](../../policies/templates/gcp_bq_dataset_location_v1.yaml)                                              |                                                                                                                                  |
| [GCPCMEKRotationConstraintV1](../../policies/templates/gcp_cmek_rotation_v1.yaml)                                                               | [cmek_rotation](../../samples/cmek_rotation.yaml)                                                                                |
| [GCPComputeExternalIpAccessConstraintV1](../../policies/templates/gcp_compute_external_ip_access_v1.yaml)                                       | [forbid_external_ip_whitelist](../../samples/vm_external_ip.yaml)                                                                |
| [GCPComputeNetworkInterfaceWhitelistConstraintV1](../../policies/templates/gcp_compute_network_interface_whitelist_v1.yaml)                     | [whitelist](../../samples/compute_network_interface_whitelist.yaml)                                                              |
| [GCPDataprocLocationConstraintV1](../../policies/templates/gcp_dataproc_location_v1.yaml)                                                       |                                                                                                                                  |
| [GCPDNSSECConstraintV1](../../policies/templates/gcp_dnssec_v1.yaml)                                                                            | [require_dnssec](../../samples/dnssec.yaml)                                                                                      |
| [GCPEnforceNamingConstraintV1](../../policies/templates/gcp_enforce_naming_v1.yaml)                                                             |                                                                                                                                  |
| [GCPGKEAllowedNodeSAConstraintV1](../../policies/templates/gcp_gke_allowed_node_sa_v1.yaml)                                                     | [gke_allowed_node_service_account_scope_default](../../samples/gke_allowed_node_sa_scope.yaml)                                   |
| [GKEClusterLocationConstraintV2](../../policies/templates/gcp_gke_cluster_location_v2.yaml)                                                     | [gke-cluster-allowed-locations](../../samples/gke_cluster_location.yaml)                                                         |
| [GCPGKEDashboardConstraintV1](../../policies/templates/gcp_gke_dashboard_v1.yaml)                                                               | [disable_gke_dashboard](../../samples/gke_dashboard_disable.yaml)                                                                |
| [GCPGKEDisableLegacyEndpointsConstraintV1](../../policies/templates/gcp_gke_disable_legacy_endpoints_v1.yaml)                                   | [disable_gke_legacy_endpoints](../../samples/gke_disable_legacy_endpoints.yaml)                                                  |
| [GCPGKEEnableStackdriverKubernetesEngineMonitoringV1](../../policies/templates/gcp_gke_enable_stackdriver_kubernetes_engine_monitoring_v1.yaml) | [enable_gke_stackdriver_kubernetes_engine_monitoring](../../samples/gke_enable_stackdriver_kubernetes_engine_monitoring.yaml)    |
| [GCPGKEEnableStackdriverMonitoringConstraintV1](../../policies/templates/gcp_gke_enable_stackdriver_monitoring_v1.yaml)                         | [enable_gke_stackdriver_monitoring](../../samples/gke_enable_stackdriver_monitoring.yaml)                                        |
| [GCPGKEMasterAuthorizedNetworksEnabledConstraintV1](../../policies/templates/gcp_gke_master_authorized_networks_enabled_v1.yaml)                | [enable_gke_master_authorized_networks](../../samples/gke_master_authorized_networks_enabled.yaml)                               |
| [GCPGKENodeAutoUpgradeConstraintV1](../../policies/templates/gcp_gke_node_auto_upgrade_v1.yaml)                                                 | [enable_auto_upgrade](../../samples/gke_node_pool_auto_upgrade.yaml)                                                             |
| [GCPGKERestrictClientAuthenticationMethodsConstraintV1](../../policies/templates/gcp_gke_restrict_client_auth_methods_v1.yaml)                  | [gke_restrict_client_auth_methods](../../samples/gke_restrict_client_auth_methods.yaml)                                          |
| [GCPIAMAllowedBindingsConstraintV1](../../policies/templates/gcp_iam_allowed_bindings_v1.yaml)                                                  | [blacklist_gmail](../../samples/iam_restrict_gmail.yaml), [blacklist_serviceaccount_user](../../samples/iam_blacklist_role.yaml) |
| [GCPIAMAuditLogConstraintV1](../../policies/templates/gcp_iam_audit_log.yaml)                                                                   | [audit_log_data_read_write](../../samples/iam_audit_log.yaml)                                                                    |
| [GCPIAMRestrictServiceAccountKeyTypeConstraintV1](../../policies/templates/gcp_iam_restrict_service_account_key_type_v1.yaml)                   | [iam_restrict_service_account_key_type](../../samples/gcp_iam_restrict_service_account_key_type.yaml)                            |
| [GCPNetworkEnableFirewallLogsConstraintV1](../../policies/templates/gcp_network_enable_firewall_logs_v1.yaml)                                   | [enable-network-firewall-logs](../../samples/network_enable_firewall_logs.yaml)                                                  |
| [GCPNetworkEnablePrivateGoogleAccessConstraintV1](../../policies/templates/gcp_network_enable_private_google_access_v1.yaml)                    | [enable_network_private_google_access](../../samples/network_enable_private_google_access.yaml)                                  |
| [GCPGKERestrictPodTrafficConstraintV1](../../policies/templates/gcp_gke_restrict_pod_traffic_v1.yaml)                                           |                                                                                                                                  |
| [GCPServiceUsageConstraintV1](../../policies/templates/gcp_serviceusage_allowed_services_v1.yaml)                                               | [allow_basic_set_of_apis](../../samples/serviceusage_allow_basic_apis.yaml)                                                      |
| [GCPSQLAllowedAuthorizedNetworksConstraintV1](../../policies/templates/gcp_sql_allowed_authorized_networks_v1.yaml)                             | [sql_allowed_authorized_networks_whitelist](../../samples/sql_allowed_authorized_networks.yaml)                                  |
| [GCPSQLInstanceTypeConstraintV1](../../policies/templates/gcp_sql_instance_type_v1.yaml)                                                        |                                                                                                                                  |
| [GCPSQLMaintenanceWindowConstraintV1](../../policies/templates/gcp_sql_maintenance_window_v1.yaml)                                              |                                                                                                                                  |
| [GCPSQLSSLConstraintV1](../../policies/templates/gcp_sql_ssl_v1.yaml)                                                                           |                                                                                                                                  |
| [GCPStorageBucketWorldReadableConstraintV1](../../policies/templates/gcp_storage_bucket_world_readable_v1.yaml)                                 | [blacklist_public_users](../../samples/storage_blacklist_public.yaml)                                                            |
| [GCPStorageLocationConstraintV1](../../policies/templates/gcp_storage_location_v1.yaml)                                                         | [allow_some_storage_location](../../samples/storage_location.yaml)                                                               |
| [GCPVPCSCEnsureAccessLevelsConstraintV1](../../policies/templates/gcp_vpc_sc_ensure_access_levels_v1.yaml)                                      | [vpc_sc_ensure_access_levels](../../samples/vpc_sc_ensure_access_levels.yaml)                                                    |
| [GCPVPCSCEnsureServicesConstraintV1](../../policies/templates/gcp_vpc_sc_ensure_services_v1.yaml)                                               | [vpc_sc_ensure_services](../../samples/vpc_sc_ensure_services.yaml)                                                              |
| [GCPVPCSCProjectPerimeterConstraintV1](../../policies/templates/legacy/gcp_vpc_sc_project_perimeter_v1.yaml)                                    | [vpc_sc_project_perimeter_blacklist](../../samples/vpc_sc_project_perimeter_v1_blacklist.yaml)                                   |
| [GCPVPCSCWhitelistRegionsConstraintV1](../../policies/templates/gcp_vpc_sc_whitelist_regions_v1.yaml)                                           | [vpc_sc_whitelist_regions](../../samples/vpc_sc_whitelist_regions.yaml)                                                          |

## Sample Constraints

The repo also contains a number of sample constraints:

| Sample                                                                                                                        | Template                                                                                                                                        | Description                                                                       |
| ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| [deny_some_resource_types](../../samples/allowed_resource_types.yaml)                                                         |                                                                                                                                                 |                                                                                   |
| [service_versions](../../samples/appengine_versions.yaml)                                                                     |                                                                                                                                                 |                                                                                   |
| [gcp-bq-cmek-encryption-v1](../../samples/bigquery_cmek.yaml)                                                                 |                                                                                                                                                 |                                                                                   |
| [require_bq_table_iam](../../samples/bigquery_world_readable.yaml)                                                            |                                                                                                                                                 |                                                                                   |
| [cmek_rotation](../../samples/cmek_rotation.yaml)                                                                             | [GCPCMEKRotationConstraintV1](../../policies/templates/gcp_cmek_rotation_v1.yaml)                                                               |                                                                                   |
| [forbid_external_ip_whitelist](../../samples/vm_external_ip.yaml)                                                             | [GCPComputeExternalIpAccessConstraintV1](../../policies/templates/gcp_compute_external_ip_access_v1.yaml)                                       |                                                                                   |
| [whitelist](../../samples/compute_network_interface_whitelist.yaml)                                                           | [GCPComputeNetworkInterfaceWhitelistConstraintV1](../../policies/templates/gcp_compute_network_interface_whitelist_v1.yaml)                     |                                                                                   |
| [require_dnssec](../../samples/dnssec.yaml)                                                                                   | [GCPDNSSECConstraintV1](../../policies/templates/gcp_dnssec_v1.yaml)                                                                            |                                                                                   |
| [dnssec_prevent_rsasha1_zsk](../../samples/dnssec_prevent_rsasha1_zsk.yaml)                                                   |                                                                                                                                                 | Ensure that RSASHA1 is not used for zone-signing key in Cloud DNS                 |
| [require_labels](../../samples/enforce_label.yaml)                                                                            |                                                                                                                                                 |                                                                                   |
| [gke_allowed_node_service_account_scope_default](../../samples/gke_allowed_node_sa_scope.yaml)                                | [GCPGKEAllowedNodeSAConstraintV1](../../policies/templates/gcp_gke_allowed_node_sa_v1.yaml)                                                     |                                                                                   |
| [disable_gke_dashboard](../../samples/gke_dashboard_disable.yaml)                                                             | [GCPGKEDashboardConstraintV1](../../policies/templates/gcp_gke_dashboard_v1.yaml)                                                               | Ensure Kubernetes web UI / Dashboard is disabled                                  |
| [disable_gke_legacy_endpoints](../../samples/gke_disable_legacy_endpoints.yaml)                                               | [GCPGKEDisableLegacyEndpointsConstraintV1](../../policies/templates/gcp_gke_disable_legacy_endpoints_v1.yaml)                                   |                                                                                   |
| [enable_gke_stackdriver_kubernetes_engine_monitoring](../../samples/gke_enable_stackdriver_kubernetes_engine_monitoring.yaml) | [GCPGKEEnableStackdriverKubernetesEngineMonitoringV1](../../policies/templates/gcp_gke_enable_stackdriver_kubernetes_engine_monitoring_v1.yaml) | Ensure Stackdriver Kubernetes Engine Monitoring is enabled                        |
| [enable_gke_stackdriver_monitoring](../../samples/gke_enable_stackdriver_monitoring.yaml)                                     | [GCPGKEEnableStackdriverMonitoringConstraintV1](../../policies/templates/gcp_gke_enable_stackdriver_monitoring_v1.yaml)                         | Ensure stackdriver monitoring is enabled on a GKE cluster                         |
| [enable_gke_master_authorized_networks](../../samples/gke_master_authorized_networks_enabled.yaml)                            | [GCPGKEMasterAuthorizedNetworksEnabledConstraintV1](../../policies/templates/gcp_gke_master_authorized_networks_enabled_v1.yaml)                | Ensure Master authorized networks is set to Enabled on Kubernetes Engine Clusters |
| [enable_auto_upgrade](../../samples/gke_node_pool_auto_upgrade.yaml)                                                          | [GCPGKENodeAutoUpgradeConstraintV1](../../policies/templates/gcp_gke_node_auto_upgrade_v1.yaml)                                                 | Ensure Automatic node upgrades is enabled on Kubernetes Engine Clusters nodes     |
| [gke_restrict_client_auth_methods](../../samples/gke_restrict_client_auth_methods.yaml)                                       | [GCPGKERestrictClientAuthenticationMethodsConstraintV1](../../policies/templates/gcp_gke_restrict_client_auth_methods_v1.yaml)                  |                                                                                   |
| [glb_external_ip_allowlist](../../samples/gcp_glb_external_ip.yaml)                                                           |                                                                                                                                                 |                                                                                   |
| [iam_ban_roles](../../samples/iam_banned_roles.yaml)                                                                          |                                                                                                                                                 | Only the roles in this list trigger violation. All other roles allowed.           |
| [blacklist_gmail](../../samples/iam_restrict_gmail.yaml)                                                                      | [GCPIAMAllowedBindingsConstraintV1](../../policies/templates/gcp_iam_allowed_bindings_v1.yaml)                                                  | Enforce corporate domain by banning gmail.com addresses                           |
| [blacklist_serviceaccount_user](../../samples/iam_blacklist_role.yaml)                                                        | [GCPIAMAllowedBindingsConstraintV1](../../policies/templates/gcp_iam_allowed_bindings_v1.yaml)                                                  | Ban any users from being granted Service Account User access                      |
| [only_my_domain](../../samples/iam_restrict_domain.yaml)                                                                      |                                                                                                                                                 | Only allow members from my domain to added to IAM roles                           |
| [audit_log_data_read_write](../../samples/iam_audit_log.yaml)                                                                 | [GCPIAMAuditLogConstraintV1](../../policies/templates/gcp_iam_audit_log.yaml)                                                                   |                                                                                   |
| [iam_restrict_service_account_key_type](../../samples/gcp_iam_restrict_service_account_key_type.yaml)                         | [GCPIAMRestrictServiceAccountKeyTypeConstraintV1](../../policies/templates/gcp_iam_restrict_service_account_key_type_v1.yaml)                   |                                                                                   |
| [enable-network-firewall-logs](../../samples/network_enable_firewall_logs.yaml)                                               | [GCPNetworkEnableFirewallLogsConstraintV1](../../policies/templates/gcp_network_enable_firewall_logs_v1.yaml)                                   | Ensure Firewall logs is enabled for every firewall in VPC Network                 |
| [enable_network_private_google_access](../../samples/network_enable_private_google_access.yaml)                               | [GCPNetworkEnablePrivateGoogleAccessConstraintV1](../../policies/templates/gcp_network_enable_private_google_access_v1.yaml)                    | Ensure Private Google Access is enabled for all subnetworks in VPC                |
| [restrict-firewall-rule-allow-ingress-demo](../../samples/restrict_fw_rules_generic.yaml)                                     |                                                                                                                                                 |                                                                                   |
| [restrict-firewall-rule-ssh-world-open](../../samples/restrict_fw_rules_ssh_world_open.yaml)                                  |                                                                                                                                                 |                                                                                   |
| [sql_allowed_authorized_networks_whitelist](../../samples/sql_allowed_authorized_networks.yaml)                               | [GCPSQLAllowedAuthorizedNetworksConstraintV1](../../policies/templates/gcp_sql_allowed_authorized_networks_v1.yaml)                             |                                                                                   |
| [gcp-sql-backup-with-exemptions](../../samples/sql_backup_with_exemptions.yaml)                                               |                                                                                                                                                 |                                                                                   |
| [allow_some_sql_location](../../samples/sql_location.yaml)                                                                    |                                                                                                                                                 |                                                                                   |
| [prevent-public-ip-cloudsql](../../samples/sql_public_ip.yaml)                                                                |                                                                                                                                                 | Prevents a public IP from being assigned to a Cloud SQL instance.                 |
| [allow_basic_set_of_apis](../../samples/serviceusage_allow_basic_apis.yaml)                                                   | [GCPServiceUsageConstraintV1](../../policies/templates/gcp_serviceusage_allowed_services_v1.yaml)                                               | Only a basic set of APIS                                                          |
| [allow_spanner_clusters_in_asia_and_europe](../../samples/spanner_location.yaml)                                              |                                                                                                                                                 |                                                                                   |
| [blacklist_public_users](../../samples/storage_blacklist_public.yaml)                                                         | [GCPStorageBucketWorldReadableConstraintV1](../../policies/templates/gcp_storage_bucket_world_readable_v1.yaml)                                 | Prevent public users from having access to resources via IAM                      |
| [allow_some_storage_location](../../samples/storage_location.yaml)                                                            | [GCPStorageLocationConstraintV1](../../policies/templates/gcp_storage_location_v1.yaml)                                                         |                                                                                   |
| [vpc_sc_ensure_access_levels](../../samples/vpc_sc_ensure_access_levels.yaml)                                                 | [GCPVPCSCEnsureAccessLevelsConstraintV1](../../policies/templates/gcp_vpc_sc_ensure_access_levels_v1.yaml)                                      |                                                                                   |
| [vpc_sc_ensure_services](../../samples/vpc_sc_ensure_services.yaml)                                                           | [GCPVPCSCEnsureServicesConstraintV1](../../policies/templates/gcp_vpc_sc_ensure_services_v1.yaml)                                               |                                                                                   |
| [vpc_sc_project_perimeter_blacklist](../../samples/vpc_sc_project_perimeter_v1_blacklist.yaml)                                | [GCPVPCSCProjectPerimeterConstraintV1](../../policies/templates/legacy/gcp_vpc_sc_project_perimeter_v1.yaml)                                    |                                                                                   |
| [vpc_sc_project_perimeter_blacklist](../../samples/vpc_sc_project_perimeter_blacklist.yaml)                                   |                                                                                                                                                 |                                                                                   |
| [vpc_sc_whitelist_regions](../../samples/vpc_sc_whitelist_regions.yaml)                                                       | [GCPVPCSCWhitelistRegionsConstraintV1](../../policies/templates/gcp_vpc_sc_whitelist_regions_v1.yaml)                                           |                                                                                   |
| [gke-cluster-allowed-locations](../../samples/gke_cluster_location.yaml)                                                      | [GKEClusterLocationConstraintV2](../../policies/templates/gcp_gke_cluster_location_v2.yaml)                                                     |                                                                                   |