---
ms.service: azure-monitor
ms.topic: include
ms.date: 08/28/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: NCBMSystemLogs
---


| Column | Type | Description |
|---|---|---|
| _BilledSize | real | The record size in bytes |
| ClusterManagerName | string | Name of the ClusterManager managing the Nexus cluster. |
| ClusterName | string | Name of the on-prem Nexus cluster. |
| Facility | string | Log facility type. E.g. daemon, kern, syslog, user. |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is `false` ingestion isn't billed to your Azure account |
| Location | string | Location of the Nexus Baremetal machine. |
| Message | string | Syslog message generated by the Baremetal machine. |
| Node | string | Host name of the Baremetal Machine. |
| ProcessId | int | ID of the process emitting the log. |
| ProcessName | string | Identification of the process generating the log. |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| Severity | string | Severity of the log record. E.g. Info, Warning, Critical, Error, Notice, Debug. |
| SourceSystem | string | The type of agent the event was collected by. For example, `OpsManager` for Windows agent, either direct connect or Operations Manager, `Linux` for all Linux agents, or `Azure` for Azure Diagnostics |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string | The Log Analytics workspace ID |
| TimeGenerated | datetime | Timestamp (UTC) when the log was generated. |
| Type | string | The name of the table |
