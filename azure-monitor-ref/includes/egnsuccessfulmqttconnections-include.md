---
ms.service: azure-monitor
ms.topic: include
ms.date: 12/11/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: EGNSuccessfulMqttConnections
---


| Column | Type | Description |
|---|---|---|
| AuthenticationType | string | Type of authentication used by the client. |
| _BilledSize | real | The record size in bytes |
| ClientIdentity | string | Value of the client's identity. |
| ClientIdentitySource | string | Source of the identity of the client issuing the request. |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is `false` ingestion isn't billed to your Azure account |
| OperationName | string | The name of the operation. |
| Protocol | string | Protocol used by the client to connect. Possible values are: MQTT3, MQTT3-WS, MQTT5, MQTT5-WS. |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| SessionName | string | Name of the session provided by the client in the MQTT CONNECT packet's clientId field. |
| SourceSystem | string | The type of agent the event was collected by. For example, `OpsManager` for Windows agent, either direct connect or Operations Manager, `Linux` for all Linux agents, or `Azure` for Azure Diagnostics |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string | The Log Analytics workspace ID |
| TimeGenerated | datetime | Timestamp (UTC) when the log was generated. |
| Type | string | The name of the table |
