---
ms.service: azure-monitor
ms.topic: include
ms.date: 12/04/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: AOIStorage
---


| Column | Type | Description |
|---|---|---|
| AccessTier | string | The access tier of the storage account. |
| AccountName | string | The name of the storage account. |
| AuthenticationHash | string | The hash of authentication token. |
| AuthenticationType | string | The type of authentication that was used to make the request. |
| AuthorizationDetails | dynamic | Detailed policy information used to authorize the request. |
| _BilledSize | real | The record size in bytes |
| CallerIpAddress | string | The IP address of the requester, including the port number. |
| Category | string | The category to which this row belongs to, it will be one of Ingestion, IngestionDelete or ReadStorage. |
| ClientRequestId | string | The x-ms-client-request-id header value of the request. |
| ConditionsUsed | string | A semicolon-separated list of key-value pairs that represent a condition. |
| ContentLengthHeader | long | The value of the Content-Length header for the request sent to the storage service. |
| CorrelationId | string | The ID that is used to correlate logs across resources. |
| DestinationUri | string | Records the destination URI for operations. |
| DurationMs | real | The total time, expressed in milliseconds, to perform the requested operation. This includes the time to read the incoming request, and to send the response to the requester. |
| Etag | string | The ETag identifier for the returned object, in quotes. |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is `false` ingestion isn't billed to your Azure account |
| LastModifiedTime | datetime | The Last Modified Time (LMT) for the returned object. This field is empty for operations that can return multiple objects. |
| Location | string | The location of storage account. |
| MetricResponseType | string | Records the metric response for correlation between metrics and logs. |
| ObjectKey | string | The key of the requested object, in quotes. |
| OperationCount | int | The number of each logged operation that is involved in the request. This count starts with an index of 0. Some requests require more than one operation, such as a request to copy a blob. Most requests perform only one operation. |
| OperationName | string | The type of REST operation that was performed. |
| OperationVersion | string | The storage service version that was specified when the request was made. This is equivalent to the value of the x-ms-version header. |
| Protocol | string | The protocol that is used in the operation. |
| ReferrerHeader | string | The Referer header value. |
| RehydratePriority | string | The priority used to rehydrate an archived blob. |
| RequestBodySize | long | The size of the request packets, expressed in bytes, that are read by the storage service. If a request is unsuccessful, this value might be empty. |
| RequesterAppId | string | The Open Authorization (OAuth) application ID that is used as the requester. |
| RequesterAudience | string | The OAuth audience of the request. |
| RequesterObjectId | string | The OAuth object ID of the requester. |
| RequesterTenantId | string | The OAuth tenant ID of identity. |
| RequesterTokenIssuer | string | The OAuth token issuer. |
| RequesterUpn | string | The User Principal Names of requestor. |
| RequestHeaderSize | long | The size of the request header expressed in bytes. If a request is unsuccessful, this value might be empty. |
| RequestMd5 | string | The value of either the Content-MD5 header or the x-ms-content-md5 header in the request. The MD5 hash value specified in this field represents the content in the request. |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| ResponseBodySize | long | The size of the response packets written by the storage service, in bytes. If a request is unsuccessful, this value may be empty. |
| ResponseHeaderSize | long | The size of the response header expressed in bytes. If a request is unsuccessful, this value might be empty. |
| ResponseMd5 | string | The value of the MD5 hash calculated by the storage service. |
| SasExpiryStatus | string | Records any violations in the request SAS token as per the SAS policy set in the storage account. Ex: longer SAS token duration specified than allowed per SAS policy. |
| SchemaVersion | string | The schema version of the log. |
| ServerLatencyMs | real | The total time expressed in milliseconds to perform the requested operation. This value doesn't include network latency (the time to read the incoming request and send the response to the requester). |
| ServiceType | string | The service associated with this request. |
| SourceAccessTier | string | The source tier of the storage account. |
| SourceSystem | string | The type of agent the event was collected by. For example, `OpsManager` for Windows agent, either direct connect or Operations Manager, `Linux` for all Linux agents, or `Azure` for Azure Diagnostics |
| SourceUri | string | Records the source URI for operations. |
| StatusCode | string | The HTTP status code for the request. If the request is interrupted, this value might be set to Unknown. |
| StatusText | string | The status of the requested operation. |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string | The Log Analytics workspace ID |
| TimeGenerated | datetime | The time (UTC) at which this event was generated. |
| TlsVersion | string | The TLS version used in the connection of request. |
| Type | string | The name of the table |
| Uri | string | Uniform resource identifier that is requested. |
| UserAgentHeader | string | The User-Agent header value, in quotes. |
